---
title: Designer
permalink: /docs/designer-overview/
---

<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. Each <code>component</code> basically is a pair of HTML <code>Template</code> and Javascript <code>ViewModel</code>, and it produces instance of <code>MVVM runtime model</code>.
<br/>
<br/>
<code>SPA Forms 365 Designer</code> is a multipage development environment, where <code>one page</code> surfaces a <code>single component</code> at SPA Form project. Each Designer page appears as individual <code>TAB</code> with <code>ribbon</code>. Caption on tab indicates component <code>name</code>.
### Designer Page
Windows with component Template, Model and MVVM Layout editors occupied largest area on page, along with set of design controls residing on <code>ribbon</code>. All component-related areas on screenshot below are indicated  with <code class="option">green border</code>. 
<br/>
<br/>
Along with <code>component management</code> controls, <code>ribbon</code> has set of controls for <code>SPA Form project</code> management. These groups of controls on screenshot are highlighted with <code class="project">red border</code> . 
<br/>
<br/>
![Image of Designer Page](/img/designer-page2.png)

### Component Management Controls
![Image of Editors](/img/Editors.png) To design and debug component, developer can use Ribbon to toggle up to 3 editors: <code>HTML Template</code>, <code>Javascript Model</code> and <code>HTML Layout</code>.    
<br/>
![Image of Designer Overview](/img/form-designer3.gif)
<br/>
The <code>HTML Template</code> & <code>Javascript Model</code> are full-fledged editors, powered with <b>[Ace code editor](https://ace.c9.io/#nav=about){:target="_blank"}</b>. These editors are matching features and performance of native editors such as Sublime, Vim and TextMate. 
<br/>

![Image of Grid](/img/Grid.png) The <code>HTML Layout</code> represents MVVM model visualization at runtime and provides complimentary interactive visual editing support for HTML Template. The <code>Grid</code> button on Ribbon toggles <code>HTML Layout</code> editor between graphical design and visualization modes. 
<br/>

![Image of Run](/img/Run.png) During development code changes are stored <code>in memory</code> and either automatically visualized at HTML Layout window or can be forcible refreshed using <code>Run</code> button on Ribbon.
<br/>

![Image of UndoRedo](/img/UndoRedo.png) <code>Undo</code> and <code>Redo</code> buttons on Ribbon are shared between components's Template and Model and applied for an editor currently <code>in focus</code>. 
<br/>

### Project Management Controls
![Image of Open](/img/Open.png) To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>

![Image of Components](/img/Components.png) To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>

![Image of Publish](/img/Publish.png) To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>

![Image of Upload](/img/Upload.png) To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>

![Image of Versions Control](/img/VersionsControl.png) Current source for a whole component (including template, model and dependencies) can be saved as a new <code>version</code> into remote <code>GitHub</code> repository. Use <code>Version Control</code> button on Ribbon to access <code>Versions History</code> panel to manage component versions. 
<br/>

![Image of Browse](/img/Browse.png) To remotely browse SPA Form project source folder on SharePoint server with Windows Explorer on your local computer use <code>Explore Files</code> button on Ribbon. Then you can use any regular editor for code editing. Notepad++ or Visual Studio Code are recommended editors: you can close Windows Explorer window, but stay connected with these editors. 
<div class="note warning">
  <h5>Explore Files works only with Internet Explorer.</h5>
  <p>
    In the meantime only <code>Internet Explorer</code> enables remote connectivity feature. You may (recommended !) routinely use modern web browser (like Google Chrome or Microsoft Edge), and use Internet Explorer occasionally - just to open project source code folder in Windows Explorer.
  </p>
</div>

To get help or support information, prress <code>Support</code> button located at the right edge of the Ribbon. 
![Image of Support](/img/Support.png) To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>


<div class="mobile-side-scroller" style="display:none;">
<table>
  <thead>
    <tr>
      <th>RIBBON CONTROL</th>
      <th><span class="filter">FUNCTIONAL</span> and <span class="output">DESCRIPTION</span></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="align-center">
        <p class="name"><strong>Relative URL</strong></p>
      </td>
      <td >
        <p>
        <code>Undo</code> and <code>Redo</code> buttons on Ribbon are shared between components's Template and Model and applied for an editor currently <code>in focus</code>.         
        </p>
      </td>
    </tr>
    <tr>
      <td class="align-center">
        <p class="name"><strong>Relative URL</strong></p>
      </td>
      <td >
        <p>
        To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks.         
        </p>
      </td>
    </tr>
    <tr>
      <td class="align-center">
        <p class="name"><strong>Relative URL</strong></p>
      </td>
      <td >
        <p>
        Current source for a whole component (including template, model and dependencies) can be saved as a new <code>version</code> into remote <code>GitHub</code> repository. Use <code>Version Control</code> button on Ribbon to access <code>Versions History</code> panel to manage component versions.          
        </p>
      </td>
    </tr>
    <tr>
      <td class="align-center">
        <p class="name"><strong>Relative URL</strong></p>
      </td>
      <td >
        <p>
        To remotely browse SPA Form project source folder on SharePoint server with Windows Explorer on your local computer use <code>Explore Files</code> button on Ribbon. Then you can use any regular editor for code editing. Notepad++ or Visual Studio Code are recommended editors: you can close Windows Explorer window, but stay connected with these editors.          
        </p>
      </td>
    </tr>
    <tr>
      <td class="align-center">
        <p class="name"><strong>Relative URL</strong></p>
      </td>
      <td >
        <p>
        To get help or support information, prress <code>Support</code> button located at the right edge of the Ribbon.          
        </p>
      </td>
    </tr>
  </tbody>
</table>
</div>
