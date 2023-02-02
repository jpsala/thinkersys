/*
```javascript
*/

const elements = ea.getViewSelectedElements().filter(e => e.type === 'image');
if(elements.length < 2) return

let firstEl = elements[0]
elements.forEach(el => {
  if(el.y < firstEl.y) firstEl = el
})
const align = true
const changeTop = true 
let lastEl = firstEl

elements.forEach(el => {
  if(el === firstEl) return

  if(changeTop) el.y = lastEl.y + lastEl.height + 15
  
  const ratio = firstEl.width / el.width;
  const newHeight = el.height * ratio;
  el.width = firstEl.width
  el.height = newHeight
  
  if(align) el.x = firstEl.x

  lastEl = el
});
const api = ea.getExcalidrawAPI()
api.selectElements([])
await ea.addElementsToView(false,true);
