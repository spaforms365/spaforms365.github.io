---
title: Concepts and Features
permalink: /docs/structure/
---

### SPA Forms for SharePoint
#### Technology features {#technology}

* SPA Forms converts out-of-box list forms into <code>Single Page Application</code> (SPA) Forms project executed on client side: in a web browser.  SPA is a great environment to design full-fledged application on top of SharePoint list form, containing custom workflows, various visual forms and utilizing out-of-box list item as data-storage device.
* SPA Forms project's SPA is based on <b>[Knockout](http://knockoutjs.com/documentation/introduction.html){:target="_blank"}</b> <code>MVVM</code> data model. The project structured as hierarchy of a self-contained and reusable chunks: <code>components</code>. This pattern is beneficial for large applications, because it simplifies development through clear organization and encapsulation, and helps to improve runtime performance by incrementally loading (via <code>AMD</code>) application code as needed.
* SPA Form <code>Designer</code> enables visual form layout design, transparently rendered into SPA project source code. Drawing surface of the form layout is based on 2-dimensional <code>responsive grid</code>, hosting on it's cells other library or custom components. When Developer interactively places SharePoint ListItem Columns on drawing surface, Designer picks rendering library component for the column-type and injects component into hierarchy of SPA Forms project. 
* Visual appearance of SPA Form layouts and library of system components is powered with <b>[Office UI Fabric](https://dev.office.com/fabric){:target="_blank"}</b> front-end framework, ensuring building experiences that fit seamlessly into Office and Office 365.
* SPA Form Designer helps manage SPA Form project and makes it extensible via user-developed custom components. Designer provides <code>scaffolding</code> support for newly creating <code>custom components</code>, reusing system library components as a base 'class'. Custom component basically is <b>[Knockout component](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b> extended with <code>metadata</code>. SPA Form Designer uses metadata when injects component into hierarchical project model and to ensure component's external dependencies - like list columns, workflows, etc.    
* SPA Form has built-in overall lifecycle defined at <b>[state-machine workflow](/docs/usage/#formstates){:target="_blank"}</b> and enabled via <code>buttons</code> component included into system library. 


#### Design environment features {#environment}

* SPA Form project consists of a set of source code files at design time. Source code must be published into runtime model to serve end users at production. SPA Form Designer provides fully isolated from each other <code>Design</code> and <code>Runtime</code> environments. User can safely modify design and debug SPA Form project, with no risk to affect current (in use) runtime version of SPA form model. Provided publishing process supports source code build optimizaton and minification for execution on production.
* SPA Form Designer provides full-fledged form <b>[design studio environment](/docs/designer-overview/){:target="_blank"}</b>. Enviroment enables components source code editing with syntax checks, interactive visual design and form publishing in a web browser. 
* SPA Form Designer supports interactive SPA project hierarchy development including custom components management. Designer enables built-in version control support and source control integration with GitHub. 
* SPA Forms Designer provides convenience direct access to SPA Form project source code files for editing with third party editors, like notepad++ or Visual Studio Code.
* SPA Forms runtime and system components library automatically updated on-demand with newer versions from GitHub-hosted open-source project*.

### SPA Forms Portal
* Search-technology-based user-centric forms consolidation solution
* Personalized selection for user’s available forms
* Personalized form-lifecycle tracking for user’s created form instances.
* Cross domain forms consolidation is enabled for production (published) SPA Forms.

### SPA Forms Workflows
* Out-of-box SharePoint 2013 workflows are fully compatible
* SPA Form to replace OOB workflow task form*
* SPA Form custom component (activity) to implement state-machine workflows*
* SPA Form custom component (activity) to implement “email form” workflow*

