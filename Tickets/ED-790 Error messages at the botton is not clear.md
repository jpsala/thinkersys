---
tags: active
datetime: 2023-02-09 Thu 18:37:50
ID: "ED-790"
description: "Error messages at the botton is not clear"
url: "https://theirc.atlassian.net/browse/ED-790"
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

### Links to resources
- MUI is [working on it](https://github.com/mui/material-ui/pull/31991), demo [here](https://deploy-preview-31991--material-ui.netlify.app/material-ui/react-stacked-snackbars/#api), roadmap [here](https://github.com/mui/material-ui/projects/25#card-45123037)
- https://notistack.com/v2.x/getting-started
	- The solution offered right now by MUI [here](https://mui.com/material-ui/react-snackbar/#notistack) in the Docs and in a discussion thread [here](https://github.com/mui/material-ui/issues/1824)
- [MUI preview version](https://deploy-preview-31991--material-ui.netlify.app/material-ui/react-stacked-snackbars/#api) with the stacked snackbars

- alternatives to MUI
	- [Notistack](https://notistack.com/v2.x/getting-started) (the one advised by MUI)
![](Pasted%20image%2020230209190017.png)
	- [MUI-Gotit](https://github.com/ggcaponetto/mui-gotit)
![](Pasted%20image%2020230209190038.png)

- Also it can be done manually as shown by this user [here](https://codesandbox.io/s/mui-snack-stack-jnrnwq)

### It's in the MUI roadmap:
![](Pasted%20image%2020230209190713.png)