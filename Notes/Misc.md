---
datetime: 2023-02-08 Wed 09:03:43
doc-type: note
Tags: note
---

### vs-code
- Added to settings.json
	"eslint.workingDirectories": [ "./irc-directory-react-app" ] for eslint to work
- Changed in package.json
	"lint-fix": "eslint --fix 'src/**/*.{ts,tsx}'",
	"lint-check": "eslint 'src/**/*.{ts,tsx}'",
	to
	"lint-fix": "eslint --fix \"src/**/*.{ts,tsx}\"",
	"lint-check": "eslint \"src/**/*.{ts,tsx}\"",
