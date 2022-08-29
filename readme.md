# Introduction

> NOTE: This document is a work in progress. You are invented to contribute to it! 

This project is a template to start new [AsciiDoc](https://asciidoc.org/) projects using the building tool [https://asciidoctor.org/](insert_link_here).

This document will explain how you can be prepared to initialize your own AsciiDoc project.

To a complete guide on how to write AsciiDoc files see the [AsciiDoc Writer’s Guide](https://asciidoctor.org/docs/asciidoc-writers-guide/)

---

# Dependencies

Before following below steps you need to assure you have [Nodejs](https://nodejs.org/en/) and [git](https://git-scm.com/downloads) installed in your machine.

Probabbly you want to use a modern code editor as [Visual Studio Code](https://code.visualstudio.com/) to edit your AsciiDoc with proper [Asciidoc plugin installed](https://marketplace.visualstudio.com/items?itemName=asciidoctor.asciidoctor-vscode), but this project is editor agnostic and it not assumes you are using Visual Studio Code as your editor. You can choose any editor like basic [Windows Notepad](https://en.wikipedia.org/wiki/Windows_Notepad), the old traditional [vim](https://www.vim.org/), [notepad++](https://notepad-plus-plus.org/downloads/), or any other of your preference.

# Clone the repository

First of all copy the tip of the official repository from github using [tiged](https://github.com/tiged/tiged) command line where `my_project_name` is the name of your project and can be any valid folder name:


```powershell
> npx tiged https::\\github.com\link_to_the_template_respository my_project_name
> cd my_project_name 
```

---

# Build pdf document

Edit the adoc entry point which is in `./src/main.adoc` file.

> NOTE: Currently it's not recommended you  to change the name of the entry point file.

When you want do compile your pdf use the following command when you are in the project folder:

```powershell
> npm run make_pdf
```

The output file will be placed in the `.\build` directory

# Build html document

You can create also an html document, the proccess is similar to creade a pdf (see above), but the command changes a litte. Type instead:

```powershell
> npm run make_html
```

# Editing your document

You entry point for editing is `./src/main.adoc`.

If you use imagens, remember to put it in the folder `./src/imagens`.

The initial version of `./src/main.adoc` may be used as an example and a start-point of formating.

# Cleaning building files

To clean builded files you can clean all the sub-directory `./build` or simple type:

```Powershell
> npm run clean
```

# Additional Notes

All these scripts are described in the `package.json` file. And they all relies on npm packages `asciidoctor` and `asciidoctor-pdf`.




