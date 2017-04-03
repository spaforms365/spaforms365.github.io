---
title: Form Model
permalink: /docs/designer-model/
---

### Text box (<input>) two-ways binding to SharePoint column value

You can now render the [Knockout](http://knockoutjs.com/documentation/textinput-binding.html)

Add new <code>input</code> HTML control on SPA Form template and use <code>textInput</code> binding to <code>mytitle</code> member of SPA Form viewmodel. 
```html
<input type="text" data-bind="textInput: mytitle">
```
<br/>
Extend SPA Form viewmodel with new <code>mytitle</code> observable. New observable is <code>extended</code> to <code>listItem</code> interface and bound to <code>Title</code> column.
```javascript
this.mytitle = ko.observable().extend({ listItem: "Title" });
```
<br/>
Full code snipped for HTML Template
```html
<!-- Template -->
<div class="ms-Grid">
    <div class="ms-Grid-row">
        <div class="ms-u-lg12 ms-u-md12 ms-u-sm12 ms-Grid-col">
            <component-textbox id="4228f2e8-7d0c-4012-8a8b-ebd14e3b9335" params="'InternalName':'Title','Title':'Title','Description':'','MaxLength':255,'DefaultValue':null,'FieldTypeKind':2,'ReadOnlyField':false,'Required':true" class=""></component-textbox>
            <input type="text" data-bind="textInput: mytitle"> 
        </div>
    </div>
</div>
```
<br/>
Full code snipped for Javascript model
```javascript
/* ViewModel */
define([ 'text!./viewmodel.html'], function( htmlString) {
    function viewModel(params) {
        // +++ EDIT MODEL BELOW TO DESIGN YOUR CUSTOM SPA FORM
        this.mytitle = ko.observable().extend({ listItem: "Title" });
    }
    return { viewModel: viewModel, template: htmlString };
});
```

