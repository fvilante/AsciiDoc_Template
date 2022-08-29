# Introduction

> NOTE: This document is a work in progress. You are invented to Contribute to it!

This project is a template to start new AsciiDoc projects using the building tool [AsciiDoctor](insert_link_here).

This document will explain how you can be prepared to initialize your own AsciiDoc project.

---

# Dependencies

Before following below steps you need to assure you have [Nodejs](insert_link_here) and [git](insert_link_here) installed in your machine.

Probabbly you want to use a modern code editor as [Visual Studio Code](insert_link_here) to edit your AsciiDoc with proper [Asciidoctor plugins installed](insert_link_here), but this project is editor agnostic and it not assumes you are using Visual Studio Code as your editor. You can choose any editor like basic [Windows Notepad](insert_link_here), [vim](insert_link_here), [notepad++](insert_link_here), or any other of your preference.

# Clone the repository

First of all clone the official repository from github using this command:

NOTE_TO_FIX_IN_THIS_Document: Its better to copy just the tip of master_branch insted of the full repository!

```powershell
> clone https::\\github.com\link_to_the_template_respository my_project_name
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




