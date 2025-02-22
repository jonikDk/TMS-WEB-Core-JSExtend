# TMS-WEB-Core-JSExtend

This repository contains the complete source code for a Delphi package consisting of components designed for use within TMS WEB Core projects.  These components are wrappers (mostly) for popular JavaScript libraries. The first such component, a wrapper for [FlatPickr](https://flatpickr.js.org/), was first published along with the TMS Software Blog [post](https://www.tmssoftware.com/site/blog.asp?post=937) that relates to it, on May 17, 2022.

**Installation**

1. For the Design-Time Package, follow these steps.
- Download the repository ZIP and unzip into your usual Delphi Projects folder.
- Navigate to the Design-Time folder and load the JSExtend project.
- Using the Project Manager window, right-clcik on JSExtend.bpl and select 'Install'.
- You should see a message that components have been installed.

2. For the Run-Time files, there are (at least) two options.
- The individual Run-Time files can be added to your project directly OR
- Go to the Delphi Tools/Options... menu, and then under TMS WEB / Options / Library Path, add the Run-Time folder.

3. Add the JS and CSS CDN links to your Project.html file. There aren't any dependencies here, so if you only need one particular JS library, you can include only that set of links. For example:
```
<!-- Flatpickr -->
<script src="https://cdn.jsdelivr.net/npm/flatpickr@latest/dist/flatpickr.min.js"></script>
<link href="https://cdn.jsdelivr.net/npm/flatpickr@latest/dist/flatpickr.min.css" rel="stylesheet"/>

<!-- Luxon -->
<script src="https://cdn.jsdelivr.net/npm/luxon@latest/build/global/luxon.min.js"></script>
```
Once installed, you should be able to find the Delphi IDE components at the bottom of the Delphi Component Palette (in the JSExtend Group) when editing a TMS WEB Core TWebForm.  Drop the component onto the form and then set the Object Insepctor properties as desired, and the control should appear once the project is run.  There's not much to see directly in the IDE, as these kinds of controls are rendered entirely in HTML and CSS, using JavaScript, so the Delphi IDE is unable to render anything of much use here.

**Documentation**

Additional information about how to use each of the JSExtend elements can be found on these pages.

- [TJSFlatPickr](Documentation/TJSFlatPickr.md)
- [Luxon](Documentation/Luxon.md)

&nbsp;

## Key Dependencies
As with any modern web application, other JavaScript libraries/dependencies have been used in this project. Most of the time, this is handled via a CDN link (usually JSDelivr) in the Project.html file. In some cases, for performance or other reasons, they may be included directly.
- [TMS WEB Core](https://www.tmssoftware.com/site/tmswebcore.asp) - This is a TMS WEB Core project, after all
- [Flatpickr](https://flatpickr.js.org/) - For handling Date/Time UI
- [Luxon](https://moment.github.io/luxon/#/) - For handling date/time conversions

## Sponsor / Donate / Support
If you find this work interesting, helpful, or useful, or that it has sved you time, money, or both, please consider direclty supporting these efforts financially via [GitHub Sponsors](https://github.com/sponsors/500Foods) or donating via [Buy Me a Pizza](https://www.buymeacoffee.com/andrewsimard500). Also, be sure to check out these other [GitHub Repositories](https://github.com/500Foods?tab=repositories&q=&sort=stargazers) that may be of interest to you.
