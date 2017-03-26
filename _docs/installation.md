---
title: Installation
permalink: /docs/installation/
---

Full installation process for SPA Forms 365 Add-in is related to 3 various areas on SharePoint landscape:
* [Step 1:](#step1) Upload software distributive file <code>spaforms365.app</code> into <code>SharePoint Apps Catalog</code>. Normally this step is executed by SharePoint tenant or farm administrator to enable access to <code>SPA Forms 365 Installer App</code> for all other users.  
* [Step 2:](#step2) Add <code>SPA Forms 365 Installer App</code> on desired <code>SharePoint Web Site</code>. The Installer App should reside on web site, where target SharePoint List is located. The Installer App enables activation or removal of SPA Forms instances on any number of SharePoint Lists residing at the web site. Normally SharePoint user with Full Control level of access on web site can add Installer App on web site.  
* [Step 3:](#step3) Activate <code>Instance of SPA Forms</code> on desired <code>SharePoint List</code>. To substitute out-of-box forms with SPA Form on SharePoint list, an instance of SPA Forms application should be activated on that list. A SharePoint user with Design level of access or higher can activate or deactivate SPA Forms instances. 

### Requirements & Compatibility

* SharePoint: SPA Forms 365 software has been tested to run with on-premise versions of <code>SharePoint 2013 & 2016</code> and with <code>SharePoint Online on Office 365<code>.
* Web Browsers: SPA Forms 365 software has been tested for compatibility with <code>Google Chrome</code> and <code>Microsoft IE-11</code>. 

#### Step 1: Apps Catalog {#step1}
~ Upload software distributive file <code>spaforms365.app</code> containing SPA Forms 365 Installer App into <code>SharePoint Apps Catalog</code>.
* Office Apps Catalog: planned to be placed in a nearest future. 
* App Catalog at SharePoint Online: download software distributive file <code>spaforms365.app</code>. (TBD: provide hyperlink) and follow guidelines outlined at [Microsoft Office Support Article](https://support.office.com/en-us/article/Use-the-App-Catalog-to-make-custom-business-apps-available-for-your-SharePoint-Online-environment-0b6ab336-8b83-423f-a06b-bcc52861cba0) to upload distributive file into App Catalog.
* App Catalog at on premise SharePoint Farm: download software distributive file <code>spaforms365.app</code>. (TBD: provide hyperlink) and follow guidelines outlined at [Microsoft Technet Article](https://technet.microsoft.com/en-us/library/fp161234.aspx#AddApps) to upload distributive file into App Catalog.

#### Step 2: Deployment SPA Forms Installer on SharePoint site {#step2}
~ Add SPA Forms 365 Installer App on desired <code>SharePoint Web Site</code>.
~ Unlike out-of-box SharePoint list forms, custom SPA Form must be designed and published before first use with list data. Click on SharePoint list's <code>new item</code> menu item and SPA Forms runtime will reply with warning message, that published SPA project was not found. Click on <code>Open Form Design project</code> link to open SPA Form designer.
<br/>
<br/>
![Image of Add Installer](/img/form-addinstaller.png)
#### Step 3: Activate SPA Forms on SharePoint list {#step3}
~ Activate instance of SPA Forms on desired <code>SharePoint List</code>.
![Image of Activate Instance](/img/SPSForms365Installer1.PNG)
#### Remove SPA Forms off SharePoint list
![Image of Remove Instance](/img/form-remove.PNG)

- [NodeJS](https://nodejs.org/), or another JavaScript runtime (for CoffeeScript support).
- [Python 2.7](https://www.python.org/downloads/)

<div class="note info">
  <h5>Problems installing Jekyll?</h5>
  <p>
    Check out the <a href="../troubleshooting/">troubleshooting</a> page or
    <a href="{{ site.repository }}/issues/new">report an issue</a> so the
    Jekyll community can improve the experience for everyone.
  </p>
</div>

<div class="note info">
  <h5>Running Jekyll on Windows</h5>
  <p>
    While Windows is not officially supported, it is possible to get Jekyll running
    on Windows. Special instructions can be found on our
    <a href="../windows/#installation">Windows-specific docs page</a>.
  </p>
</div>

## Install with RubyGems

The best way to install Jekyll is via
[RubyGems](https://rubygems.org/pages/download). At the terminal prompt,
simply run the following command to install Jekyll:

```sh
$ gem install jekyll
```

All of Jekyll’s gem dependencies are automatically installed by the above
command, so you won’t have to worry about them at all.

<div class="note info">
  <h5>Installing Xcode Command-Line Tools</h5>
  <p>
    If you run into issues installing Jekyll's dependencies which make use of
    native extensions and are using macOS, you will need to install Xcode
    and the Command-Line Tools it ships with. Download them in
    <code>Preferences &#8594; Downloads &#8594; Components</code>.
  </p>
</div>

## Pre-releases

In order to install a pre-release, make sure you have all the requirements
installed properly and run:

```sh
gem install jekyll --pre
```

This will install the latest pre-release. If you want a particular pre-release,
use the `-v` switch to indicate the version you'd like to install:

```sh
gem install jekyll -v '2.0.0.alpha.1'
```

If you'd like to install a development version of Jekyll, the process is a bit
more involved. This gives you the advantage of having the latest and greatest,
but may be unstable.

```sh
$ git clone git://github.com/jekyll/jekyll.git
$ cd jekyll
$ script/bootstrap
$ bundle exec rake build
$ ls pkg/*.gem | head -n 1 | xargs gem install -l
```

## Optional Extras

There are a number of (optional) extra features that Jekyll supports that you
may want to install, depending on how you plan to use Jekyll. These extras
include LaTeX support, and the use of alternative content rendering engines.
Check out [the extras page](../extras/) for more information.

<div class="note">
  <h5>ProTip™: Enable Syntax Highlighting</h5>
  <p>
    If you’re the kind of person who is using Jekyll, then chances are you’ll
    want to enable syntax highlighting using <a href="http://pygments.org/">Pygments</a>
    or <a href="https://github.com/jayferd/rouge">Rouge</a>. You should really
    <a href="../templates/#code-snippet-highlighting">check out how to
    do that</a> before you go any farther.
  </p>
</div>

## Already Have Jekyll?

Before you start developing with Jekyll, you may want to check that you're up to date with the latest version. To find your version of Jekyll, run one of these commands:

```sh
$ jekyll --version
$ gem list jekyll
```

You can also use [RubyGems](https://rubygems.org/gems/jekyll) to find the current versioning of any gem. But you can also use the `gem` command line tool:

```sh
$ gem search jekyll --remote
```

and you'll search for just the name `jekyll`, and in brackets will be latest version. Another way to check if you have the latest version is to run the command `gem outdated`. This will provide a list of all the gems on your system that need to be updated. If you aren't running the latest version, run this command:

```sh
$ gem update jekyll
```

Now that you’ve got everything up-to-date and installed, let’s get to work!
