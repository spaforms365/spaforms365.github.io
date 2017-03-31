---
title: Concepts and Features
permalink: /docs/structure/
---

### SPA Forms for SharePoint
#### Technology features {#technology}

* SPA Forms converts out-of-box list forms into <code>Single Page Application</code> (SPA). SPA Form project executed on client side: in a web browser.  SPA is a great environment to design full-fledged application on top of SharePoint list form, containing custom workflows, various visual forms and utilizing out-of-box list item as data-storage device.
* SPA Forms project's SPA is based on <b>[Knockout](http://knockoutjs.com/documentation/introduction.html){:target="_blank"}</b> <code>MVVM</code> data model. The project structured as hierarchy of a self-contained and reusable chunks: <code>components</code>. This pattern is beneficial for large applications, because it simplifies development through clear organization and encapsulation, and helps to improve runtime performance by incrementally loading (via <code>AMD</code>) application code as needed.
* SPA Forms promotes visual form design style. Interactively made design modifications are transparently rendered into SPA form project source code. Form layout drawing surface is based on 2-dimensional <code>responsive grid</code>. Developer interactively configures form layout shape, picks and places SharePoint list item columns, library or custom components on the form. 
* Visual appearance of SPA Form layouts and library of system components is powered with <b>[Office UI Fabric](https://dev.office.com/fabric){:target="_blank"}</b> front-end framework, ensuring building experiences that fit seamlessly into Office and Office 365.
* For larger applications, SPA Forms promotes project extensibility via user-developed custom components. SPA Forms Designer provides <code>scaffolding</code> support to build new <code>custom components</code>, reusing system library components as a base 'class'. Custom component basically is <b>[Knockout component](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b> extended with <code>metadata</code>. SPA Form Designer refers metadata to properly inject component's instance into project hierarchical model and to ensure component's external dependencies - like list columns, workflows, etc.    
* SPA Form supports overall form state lifecycle management, documented as <b>[state-machine workflow](/docs/usage/#formstates)</b> and enabled via <code>buttons</code> component included into system library. 


#### Design environment features {#environment}

* SPA Form project is a set of source code files at design time. Source code must be published into runtime model to serve end users at production. SPA Form Designer operates with <code>Design</code> and <code>Runtime</code> environments, fully isolated from each other. User can safely design and debug SPA Form project, with no risk to affect current (in use) runtime version of SPA form model. Publishing process builds project source code into optimized and minified module for execution on production.
* SPA Form Designer is a full-fledged form <b>[design studio environment](/docs/designer-overview/)</b>. Designer allows components source code editing with syntax checks, interactive visual design and form publishing: all in a web browser. 
* SPA Form Designer supports interactive SPA project hierarchy development, including custom components management. Designer supports built-in version control for project components integrated with GitHub. 
* SPA Forms Designer provides convenience direct access to SPA Form project source code files for editing with third party editors, like notepad++ or Visual Studio Code.
* SPA Forms runtime and system components library automatically updated on-demand, when newer version of the product release is available on GitHub-hosted open-source repository*.

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

