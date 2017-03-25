---
title: Installation
permalink: /docs/installation/
---

Full installation process for SPA Forms 365 Add-in is related to 3 various areas on SharePoint landscape:
* [Step 1:](#step1) Upload software distributive file into <code>Apps Catalog</code>.
* [Step 2:](#step2) Add <code>SPA Forms 365 Installer App</code> on desired <code>Web Site</code>.
* [Step 3:](#step3) Activate instance of SPA Forms on desired <code>List</code>.

### Requirements

Installing Jekyll should be straight-forward if all requirements are met.
Before you start, make sure your system has the following:

- GNU/Linux, Unix, or macOS
- [Ruby](https://www.ruby-lang.org/en/downloads/) version 2.0 or above, including all development
  headers
- [RubyGems](https://rubygems.org/pages/download)
- [GCC](https://gcc.gnu.org/install/) and [Make](https://www.gnu.org/software/make/) (in case your system doesn't have them installed, which you can check by running `gcc -v` and `make -v` in your system's command line interface)

#### Step 1: Apps Catalog {#step1}
~ Upload software distributive file <code>spaforms365.app</code> containing SPA Forms 365 Installer App into <code>SharePoint Apps Catalog</code>.
#### ~ Office Apps Catalog

#### ~ App Catalog at SharePoint Online 

#### ~ App Catalog at on-premise SharePoint 

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
