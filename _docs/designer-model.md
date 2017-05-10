---
title: Model
permalink: /docs/designer-model/
---
<code>Model</code> implements SPA Form operations and behaviors at runtime. 
<br/>
<br/>
On practice, overall SPA Form MVVM model uses collection of components, and most of them are <b>[library components](/docs/designer-syslibrary/#syscomponents)</b>. Quite often you will need to design model for only one (root) component in your project and just reuse many library-provided models. 

### Designer tools for component development
To on component <code>source code</code>, Designer enables two side-by-side panels: <code>HTML Template</code> and <code>JS Model</code>.  These two areas on screenshot below are outlined under <code class="option">green border</code>.
<br/>
<br/>
Changes in code can be immediately visualized on <code>HTML Layout</code> panel. Template code changes at <code>HTML Template</code> are automatically rendered and Model code changes can be seen using <code>Run</code> button. These mentioned controls on screenshot below are outlined under <code class="project">red border</code> . 
<br/>
<br/> 
![Image of Ribbon Model](/img/form-ribbon-model.png)
<br/>
### SPA Forms Runtime Support for Models
<code>SPA Forms Runtime</code> extends <code>Knockout</code> via various binding extensions. Complete list of extensions is available at "place hyperlink here".
<br/>
<br/>
One of the <code>SPA Forms Runtime</code> binding extensions allows to associate SharePoint columns with viewmodel properties. SharePoint default content type on List is known (registered) as <code>listItem</code> interface at SPA Forms runtime. The runtime implements an <b>[extender](http://knockoutjs.com/documentation/extenders.html){:target="_blank"}</b> to augment observables for SharePoint data associations. 
<br/>
<br/>
Lets will review use of that extension at practical model development exercize below:

### Example: Two-ways binding to SharePoint column {#twowaybinding}

Two-ways binding explained at <b>[Knockout](http://knockoutjs.com/documentation/textinput-binding.html){:target="_blank"}</b> documentation as following:
<br/>
<br/>
"<i>the <code>textInput</code> binding links a text box <code>input</code> or text area <code>textarea</code> with a viewmodel property, providing two-way updates between the viewmodel property and the element’s value. Unlike the <code>value</code> binding,<code>textInput</code> provides instant updates from the DOM for all types of user input, including autocomplete, drag-and-drop, and clipboard events</i>".
<br/>
<br/>
Add new <code>input</code> HTML control on SPA Form template and use <code>textInput</code> binding to <code>mytitle</code> member of SPA Form viewmodel. 
```html
<input type="text" data-bind="textInput: mytitle">
```
Add <code>mytitle</code> property to SPA Form viewmodel. New property is Knockout observable <code>extended</code> to <code>listItem</code> interface and bound to <code>Title</code> column:
```javascript
this.mytitle = ko.observable().extend({ listItem: "Title" });
```
Full code snippet for HTML Template
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
Full code snippet for Javascript model
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
Result in action:
![Image of Two-Way Binding](/img/designer-model.gif)
<br/>


