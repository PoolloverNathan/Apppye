# Appye Script
#### Specifications for Appye Script, a pseudo-scripting language to customize Appye.
## `register`
##### Used to create apps, widgets, etc
#### Syntax:
```
register [type] [name] {
[json styled details]
}
```
#### Types:
`app`, `widget`, `js_trigger`, `proxy`, `searchEngine`
#### Name:
String value, must be put in quotation marks if a space is present in the name.
## `register app [name]`
##### Used to create apps.
#### Syntax:
```
register app [name] {
winStyle: ``, //string, contains all window info (use winbox.js stuff)
vendor: "",  //string, name of creator or something.
description: "", //string, contains info about the app.
hidden: , //boolen, should be hidden in UI. (maybe system/testing apps?)
commandLine: `` //string, contains the command line names, seperated by commas.
proxy: //boolen, attempt to proxy the app or not.
}
```
## `register widget [name]`
##### Used to create widgets.
#### Syntax:
```
register widget [name] {
html: "",  //string, HTML to inject into the page.
vendor: "",  //string, name of creator or something.
description: "", //string, contains info about the widget.
window: , //boolen, put it in a winbox.js window or not.
proxy:   //boolen, attempt to proxy the html or not.
}
```
## `register js_trigger [name]`
##### Used to trigger JS on certain commands.
#### Syntax:
```
register js_trigger [name] {
regex: , //boolen, whtnher to use regex or not.
on: "", //the command that triggers it, the wildcard '*', and regex works.
eval: "" //expression to evaulate, once triggered.
}
```


