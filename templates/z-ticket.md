<%*
const ID = await tp.system.prompt("Ticket ID:");
const description = (await tp.system.prompt("Description:")).replace('/', ' ').replace('?', ' ').replace(':', ' ').replace('&', ' ').replace(',', ' ').replace('.', ' ');
const url = `https://theirc.atlassian.net/browse/${ID}`
await tp.file.move("Tickets/" + ID + ' ' + description);
-%>
---
<% 'tags:' %> active
datetime: <% tp.date.now("YYYY-MM-DD ddd HH:mm:ss") %>
ID: "<% ID %>"
description: "<% description  %>"
url: "<% url  %>"
---
<span style="font-size: 15px; opacity:.2">last-modified:: `$=  moment(dv.current().file.mtime.toString()).format('YYMMDD HH:mm')`</span>
---
```dataviewjs
let url = dv.current().url
dv.paragraph(url === 'undefined' ? '' : url)
dv.paragraph("ID: " + dv.current().ID )
dv.paragraph("Description: " + dv.current().description )
```
---
<% tp.file.cursor() %>
