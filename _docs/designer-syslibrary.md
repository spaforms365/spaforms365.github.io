---
title: Components
permalink: /docs/designer-syslibrary/
---
<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. Each <code>component</code> basically is a pair of HTML <code>Template</code> and Javascript <code>ViewModel</code>, and it produces instance of <code>MVVM runtime model</code>.
<br/>
<br/>
At a minimum, <code>SPA Form project</code> 
### Components Library {#syscomponents}
<code>Components Library</code> used to render various SharePoint columns into <code>Form Fields</code> on <code>SPA Form Layout</code>. As illustrated below, when you pick SharePoint column by <code>name</code>, you also select <code>library component</code> mapped (compatible) to Sharepoint column's <code>data type</code>.
<br/>
Selected component then used to render SharePoint data on SPA Form Layout and provide interface for user interactions. 
<br/>
<br/>  
![Image of Components](/img/form-components.gif)
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

