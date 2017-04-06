---
title: Designer Overview
permalink: /docs/designer-overview/
---

SPA Forms 365 Designer is a multipage development environment, where <code>one page</code> surfaces a <code>single component</code> on hierarchy of SPA Form project. Each Designer page appears as an individual <code>TAB</code> on Ribbon. 
<br>
<br/>
<b>[Knockout component](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b> is a pair of HTML <code>Template</code> and Javascript <code>Model</code>. At runtime nested component receives <code>parameters</code> out of project hierarchy and dynamically binds its parts into <code>MVVM runtime model</code>. 
<br/>
<br/>
To design and debug component, developer can use Ribbon to toggle up to 3 editors: <code>HTML Template</code>, <code>Javascript Model</code> and <code>HTML Layout</code>.    
<br/>
![Image of Designer Overview](/img/form-designer3.gif)
<br/>
The <code>HTML Template</code> & <code>Javascript Model</code> are full-fledged editors, powered with <b>[Ace code editor](https://ace.c9.io/#nav=about){:target="_blank"}</b>. These editors are matching features and performance of native editors such as Sublime, Vim and TextMate. 
<br/>
<br/>
The <code>HTML Layout</code> represents MVVM model visualization at runtime and provides complimentary interactive visual editing support for HTML Template. The <code>Grid</code> button on Ribbon toggles <code>HTML Layout</code> editor between graphical design and visualization modes. 
<br/>
<br/>
During development code changes are stored <code>in memory</code> and either automatically visualized at HTML Layout window or can be forceavable refreshed by clicking at <code>Run</code> button on Ribbon.
<br/>
<br/>
<code>Undo</code> and <code>Redo</code> buttons on Ribbon are shared between components's Template and Model and applied for an editor currently <code>in focus</code>. 
<br/>
<br/>
To save both: template and model on SharePoint server, press <code>Save</code> button on Ribbon at any time. That will also reset Undo/Redo changes stacks. 
<br/>
<br/>
Current source for a whole component (including template, model and dependencies) can be saved as a new <code>version</code> into remote <code>GitHub</code> repository. Use <code>Version Control</code> button on Ribbon to access <code>Versions History</code> panel to manage component versions. 
<br/>
<br/>
To remotely browse SPA Form project source folder on SharePoint server with Windows Explorer on your local computer use <code>Explore Files</code> button on Ribbon. Then you can use any regular editor for code editing. Notepad++ or Visual Studio Code are recommended editors: you can close Windows Explorer window, but stay connected with these editors. 
<div class="note warning">
  <h5>Explore Files works only with Internet Explorer.</h5>
  <p>
    In the meantime only <code>Internet Explorer</code> enables remote connectivity feature. You may (recommended !) routinely use modern web browser (like Google Chrome or Microsoft Edge), and use Internet Explorer occasionally - just to open project source code folder in Windows Explorer.
  </p>
</div>
To get help or support information, prress <code>Support</code> button located at the right edge of the Ribbon. 

<div class="mobile-side-scroller">
<table>
  <thead>
    <tr>
      <th>Description</th>
      <th><span class="filter">Filter</span> and <span class="output">Output</span></th>
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
