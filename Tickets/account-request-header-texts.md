---
tags: active
datetime: 2023-02-07 Tue 22:11:08
ID: "account-request-header-texts"
description: ""
url: ""
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
## Description

