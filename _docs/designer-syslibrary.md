---
title: Components
permalink: /docs/designer-syslibrary/
---

### Components Library {#syscomponents}
<code>Components Library</code> helps to render various SharePoint columns into <code>Form Fields</code> on <code>SPA Form Layout</code>. As illustrated below, if you pick SharePoint column by <code>name</code>, you also select specific <code>library component</code> compatible with Sharepoint column<code>data type</code>.
<br/>
Selected component will then render SharePoint data on SPA Form Layout and support user interactions. 
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

