---
title: Components
permalink: /docs/designer-syslibrary/
---
<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. 
<br/>
### Basic Usage {#usecomponents}
To use a component you call it using <code>HTML markup</code> on caller's <code>Template</code>. Component has unique <code>tag</code> on HTML markup and set of <code>calling parameters</code> listed under <code>params</code> HTML attribute. 
<br/>
<br/>
Code snippet below demonstrates use of <code>TEXTBOX</code> library component placed on SPA Form Layout and rendering <code>Title</code> SharePoint column : 
```html
<!-- Template -->
<div class="ms-Grid">
    <div class="ms-Grid-row">
        <div class="ms-u-lg12 ms-u-md12 ms-u-sm12 ms-Grid-col">
            <component-textbox id="4228f2e8-7d0c-4012-8a8b-ebd14e3b9335" params="'InternalName':'Title','Title':'Title','Description':'','MaxLength':255,'DefaultValue':null,'FieldTypeKind':2,'ReadOnlyField':false,'Required':true" class=""></component-textbox>
        </div>
    </div>
</div>
```
### Visual Design Style {#visualcomponents}
To quickly construct SPA Form utilizing various library and custom components, <code>SPA Forms 365 Designer</code> promotes visual design style. Thus HTML Markup on caller's Template can be created easy and error free.
<br/>
<br/>
Video below demontrates example of complete design experience with the following visual design steps:
* [Step 1:](#step1) Turn <code>HTML Layout</code> panel into <code>Grid</code> mode.  
* [Step 2:](#step2) On <code>target cell</code> at form layout, outlined under <code class="option">green border</code>, click <code>Add Components</code> control to launch <code>Columns & Components</code> picker panel.  
* [Step 3:](#step3) On picker panel select SharePoint "Title" <code>column</code> along with (selectable) "textbox" column rendering <code>Form component</code> and <code>Place on Form</code>. 
* [Step 4:](#step4) Repeat similar exercise to place "buttons" <code>component</code>.
* [Step 5:](#step5) Use <code>Edit Source</code> control to open "textbox" library component's <code>source code</code> in a new <code>Tab</code> at <code>SPA Forms 365 Designer</code>.
* [Step 6:](#step6) Repeat the same exercise for "buttons" library component.
* [Step 7:](#step7) Turn off <code>Grid</code> mode on <code>HTML Layout</code> panel to preview final results.
<br/>
 
![Image of Components](/img/form-components.gif)
<br/>
<br/>
Visually placed components are <code>fully configured</code> by <code>SPA Forms 365 Designer</code>. 
<br/>
<br/>
However often a library component can be additionally tuned via it's <code>calling parameters</code>. Although component's calling parameters are directly editable at HTML Template panel, but SPA Forms 365 Designer again makes it easier with visual design style:
<br/>
<br/>
![Image of Call Parameters](/img/call_parameters1.gif)
<br/>

### Components Library {#syscomponents}
Working on form design <code>visually</code>, you are focused on <code>SharePoint columns</code> to place, but not <code>components</code>. However actually you are placing <code>rendering component</code>, suitable for SharePoint column's <code>data type</code> and <code>wiring</code> this component to the column. 
<br/>
<br/>
To render various <code>types</code> of SharePoint columns on form layout, <code>SPA Form 365 Designer</code> uses <code>library of components</code>. 
<br/>
<br/>
Selected component then used to render SharePoint data on SPA Form Layout and provide interface for user interactions. 
<div class="note">
  <h5>ProTip™: Access library component's source directly from Layout</h5>
  <p>
    List of library components mapped to SharePoint column types is not explicitly available anywhere in Designer.
    <br/>
    You are picking library component indirectly: by data type of SharePoint column. Then you can see placed component at<code>HTML Layout</code> panel and open another Tab in Designer to see component's source code. 
  </p>
</div>



<br/>
<br/> 
![Image of Component HTML](/img/form-component-html.png)


### Custom Components
Sometimes you may need either sligtly customize existing <code>system library component</code> or build your own new component from scratch. 
<br/>
<br/>
Source codes for all system library components are open-source, but for the runtime library components are packaged into <code>read-only</code> optimized and minified module <code>syscomponents.min.js</code>. Also usually it maybe challengeable to create new custom component from scratch.
<br/>
<br/>
The <code>Designer</code> can assist with effortless creation of fully functioning <code>prototype</code> for new custom component. So user can start from that and develop custom functionality.
<br/>
<br/>
![Image of Create Component](/img/createcomp.gif)

