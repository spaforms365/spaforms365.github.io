---
title: Form Template
permalink: /docs/designer-template/
---

SPA Forms promotes visual form design style. 
<br/>
Design modifications interactively made on form layout are immediately rendered into source code of component's HTML template. Updates made on template HTML source code are immediately reflected on form layout preview.
### Layout
SPA Form <code>content</code> visually organized and structured on top of suitable <code>layout</code>. SPA Form project is a hierarchy of components and <code>HTML Template</code> of the root (or underlying) component, usually represents <code>overall form layout</code>.
<br/>
<br/>
To maintain layout, HTML Template of the root component contains <code>responsive grid</code> powered by Office UI Fabric. It is easy to create desired form layout with interactive visual builder on <code>HTML Layout</code> editor. 
<br/>
<br/>
![Image of Grid Editing](/img/form-gridediting.gif)
<br/>
Interactive configured changes getting immediately captured and reflected on source code for HTML template. The same works in opposite direction: any changes made in HTML source code of the template immediately getting rendered on layout.

### Placing Content {#placingcomponents}

Designer can interactively pick and place SharePoint list columns, library or custom components on drawing surface of the form. Columns and Components <code>picker panel</code> is accessible right from <code>target cell</code> on responsive grid. Selected group of components are droppable in bulk on target cell and can be re-arranged later between other cells on the grid. 
<br/>
<br/>
![Image of Placing Components](/img/form-placingcomponents2.gif)
<br/>
<br/>
Interactively dropped component instance immediately gets injected into hierarchy of the SPA project. Columns and Components picker panel <code>dynamically matches</code> selected SharePoint Column properties and metadata-defined interface at Knockout component to determine <code>params values</code> needed to call <code>component instance</code>:
<br/>
<br/> 
![Image of Component HTML](/img/form-component-html.png)
 
### Freestyle Editing HTML Template {#editingtemplate}
Interactive visual design is good to quickly compose initial draft for template rendered by SPA Form component. HTML Template editor is convenient tool for further HTML template source code development. Changes made in code immediately gets visualized on HTML Layout: 
<br/>
<br/>
![Image of Placing HTML](/img/form-placinghtml.gif)

