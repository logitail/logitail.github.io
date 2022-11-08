# logitail.github.io

## 1. FOLDER STRUCTURE

Logitail is working with SDF  
the folder structure for suitescripts and SCA projects is the current standard.  
installation guide:
https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156026236161.html

or:
https://marketplace.visualstudio.com/items?itemName=Oracle.suitecloud-vscode-extension

example folder structure:
```console
[Client] > src > Filecabinet > Suitescripts > 
[feature]
- file.js
- README.md
- components.md
```
___
## 2. FILE NAMING CONVENTION

Type suitescript:

- client script - cl
- user event script - ue
- map/reduce script - mr
- mass update script - mu
- portlet script - pl
- restlet script - rl
- suitelet script - sl
- scheduled script - ss
- workflow action script - wf
- sdf installation script - si
- bundle installation script - bi

https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387172495.html

```console
[type suitescript] _ [descriptive name].js
```
1. when installing script into NetSuite use the the exact same name for the script id and the deployment id.
2. use the details in the README file for the description or suitescripts/custom records
___
## 3. SUITESCRIPT BUILD

standard JSDoc setup:
```js
/**
 * @NApiVersion 2.1 (required)
 * @NScriptType UserEventScript (type suitescript)
 * @author NAME_AUTHOR
 * @name NAME_FILE
 * @description This script triggers on after submit of Item Fullfillment record and create/update Journal Entry for each line of fullfillment.
 * @version 1.1.0 (X.0.0 major change, 1.X.0 minor change, 1.1.X small change)
 * @copyright Logitail 2020. All rights reserved.
 */
```

### CODE/COMMENTS

- elaborate 3rd party libraries: docs, link, ...
- consice commenting
- use //TODO and //FIXME tags for open tasks in code


___
## README MARKDOWN DOCUMENT
Placing a technical document (README.md) is required when creating features.  
This will come in handy when filling in the description of custom fields, suitescripts and other custom records.


See [README-sample.md](/README-sample.md) for the example file template.  
  
please refer to [Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet/) for details
___
### ABBREVIATION
|short|description|
|---|---|
| SDF | SuiteCloud Development Framework | 
| NS | NetSuite |
