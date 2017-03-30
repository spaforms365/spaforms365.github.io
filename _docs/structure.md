---
title: Concepts and Features
permalink: /docs/structure/
---

### SPA Forms for SharePoint
Technology features:

* SPA Forms converts out-of-box list forms into <code>Single Page Application</code> (SPA) Forms project executed on client side: in a web browser.  SPA is a great environment to design full-fledged application on top of SharePoint list form, containing custom workflows, various visual forms and utilizing out-of-box list item as data-storage device.
* SPA Forms project's SPA is based on <b>[Knockout](http://knockoutjs.com/documentation/introduction.html){:target="_blank"}</b> <code>MVVM</code> data model. The project structured as hierarchy of a self-contained and reusable chunks: <code>components</code>. This pattern is beneficial for large applications, because it simplifies development through clear organization and encapsulation, and helps to improve runtime performance by incrementally loading (via <code>AMD</code>) application code as needed.
* SPA Form <code>Designer</code> enables visual form layout design, transparently rendered into SPA project source code. Drawing surface of the form layout is based on 2-diminsional <code>responsive grid</code>, hosting on it's cells other library or custom components. When Developer interactively places Columns of SharePoint ListItem on drawing surface, Designer picks rendering library component for that column-type and injects component into hierarchy of SPA Forms project. 
* Visual appearance of SPA Form layouts and library of system components is powered with <b>[Office UI Fabric](https://dev.office.com/fabric){:target="_blank"}</b> front-end framework, ensuring building experiences that fit seamlessly into Office and Office 365.
* SPA Form Designer helps manage SPA Form project and makes it extensible via user-developed custom components. Designer provides <code>scaffolding</code> support for newly creating <code>custom components</code>, reusing system library components as a base 'class'. Custom component basically is Knockout component with extended <code>metadata</code>. SPA Form Designer uses metadata when injects component into hierarchical project model and to ensure component's external dependencies - like list columns, workflows, etc.    
* SPA Form has built-in overall lifecycle defined as state-machine workflow and enabled via <code>buttons</code> component included into system library. 


SPA FORMS 365 Product features

* At design time, custom SPA Form project is a set of source code files. Source code should be published into runtime model serving end users at production. SPA Form Designer provides fully isolated from each other <code>Design</code> and <code>Runtime</code> environments. User can safely modify design and debug SPA Form project, with no risk to affect current (in use) runtime version of SPA form model. Provided publishing process supports source code build optimizaton and minification for execution on production.
* Integrated web-based form design studio:
* Graphical web-based form designer (design on top of alive form data).
* Custom components management.
* Web-based editors for components with code-syntax checks.
* Built-in source control integration (GitHub & under development: TFS server).
* Direct form & components code editing with any editor (notepad++)
* Runtime and base components library updated on-demand with newer versions from GitHub-hosted open-source project*.

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

<div class="mobile-side-scroller">
<table>
  <thead>
    <tr>
      <th>File / Directory</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <p><code>_config.yml</code></p>
      </td>
      <td>
        <p>
          Stores <a href="../configuration/">configuration</a> data. Many of
          these options can be specified from the command line executable but
          it’s easier to specify them here so you don’t have to remember them.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_drafts</code></p>
      </td>
      <td>
        <p>
          Drafts are unpublished posts. The format of these files is without a
          date: <code>title.MARKUP</code>. Learn how to <a href="../drafts/">
          work with drafts</a>.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_includes</code></p>
      </td>
      <td>
        <p>
          These are the partials that can be mixed and matched by your layouts
          and posts to facilitate reuse. The liquid tag
          <code>{% raw %}{% include file.ext %}{% endraw %}</code>
          can be used to include the partial in
          <code>_includes/file.ext</code>.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_layouts</code></p>
      </td>
      <td>
        <p>
          These are the templates that wrap posts. Layouts are chosen on a
          post-by-post basis in the
          <a href="../frontmatter/">YAML Front Matter</a>,
          which is described in the next section. The liquid tag
          <code>{% raw %}{{ content }}{% endraw %}</code>
          is used to inject content into the web page.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_posts</code></p>
      </td>
      <td>
        <p>
          Your dynamic content, so to speak. The naming convention of these
          files is important, and must follow the format:
          <code>YEAR-MONTH-DAY-title.MARKUP</code>.
          The <a href="../permalinks/">permalinks</a> can be customized for
          each post, but the date and markup language are determined solely by
          the file name.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_data</code></p>
      </td>
      <td>
        <p>
          Well-formatted site data should be placed here. The Jekyll engine
          will autoload all data files (using either the <code>.yml</code>,
          <code>.yaml</code>, <code>.json</code> or <code>.csv</code>
          formats and extensions) in this directory, and they will be
          accessible via `site.data`. If there's a file
          <code>members.yml</code> under the directory, then you can access
          contents of the file through <code>site.data.members</code>.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_sass</code></p>
      </td>
      <td>
        <p>
          These are sass partials that can be imported into your <code>main.scss</code>
          which will then be processed into a single stylesheet
          <code>main.css</code> that defines the styles to be used by your site.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>_site</code></p>
      </td>
      <td>
        <p>
          This is where the generated site will be placed (by default) once
          Jekyll is done transforming it. It’s probably a good idea to add this
          to your <code>.gitignore</code> file.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>.jekyll-metadata</code></p>
      </td>
      <td>
        <p>
          This helps Jekyll keep track of which files have not been modified
          since the site was last built, and which files will need to be
          regenerated on the next build. This file will not be included in the
          generated site. It’s probably a good idea to add this to your
          <code>.gitignore</code> file.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p><code>index.html</code> or <code>index.md</code> and other HTML,
        Markdown, Textile files</p>
      </td>
      <td>
        <p>
          Provided that the file has a <a href="../frontmatter/">YAML Front
          Matter</a> section, it will be transformed by Jekyll. The same will
          happen for any <code>.html</code>, <code>.markdown</code>,
          <code>.md</code>, or <code>.textile</code> file in your site’s root
          directory or directories not listed above.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>Other Files/Folders</p>
      </td>
      <td>
        <p>
          Every other directory and file except for those listed above—such as
          <code>css</code> and <code>images</code> folders,
          <code>favicon.ico</code> files, and so forth—will be copied verbatim
          to the generated site. There are plenty of <a href="../sites/">sites
          already using Jekyll</a> if you’re curious to see how they’re laid
          out.
        </p>
      </td>
    </tr>
  </tbody>
</table>
</div>
