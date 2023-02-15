---
tags: active
datetime: 2023-02-10 Fri 13:13:10
ID: "ED-785"
description: "Regular Employee has an End Date for the Upgrade PD  end date should be grayed out"
url: "https://theirc.atlassian.net/browse/ED-785"
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

hover on name doesn't have to change
validate end date