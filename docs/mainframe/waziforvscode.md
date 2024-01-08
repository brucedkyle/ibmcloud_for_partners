# Wazi for VS Code

**Wazi Developer for VS Code** extends the functions of **VS Code** to provide z/OS developers with a familiar and straightforward edit, build, and debug experience. VS Code is becoming the most popular development environment according to recent surveys. With so many current and next generation developers having experience with VS Code, IBM enterprise language support in VS Code makes enterprise programming more attractive and productive by allowing developers to use this popular editor, with the option to integrate numerous other extensions from the VS Code Marketplace.

## Overview

Runs on desktop. It provides a set of Microsoft VS Code extensions to extend VS Code to deliver a simple and familiar edit, build, and debug experience.

VS Code is a popular desktop editor among many current and next generation developers. IBM Enterprise language support in VS Code makes enterprise programming more attractive and productive by allowing developers to use this popular editor, with the option to integrate numerous other extensions from the VS Code Marketplace.

See [Developing with IBM Wazi for VS Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-option-1-developing-wazi-vs).

Download IBM Wazi for VS Code and then install:

- Zowe Explorer
- IBM Z Open Editor
- IBM Z Open Debug

## Zowe Explorer

The [Zowe Explorer extension for Visual Studio Code (VS Code)](https://docs.zowe.org/stable/getting-started/overview) modernizes the way developers and system administrators interact with z/OS mainframes, and lets you interact with data sets, USS files, and jobs.

You can graphically navigate and access file and job resources on z/OS by using the Zowe Explorer VS Code extension. It is recommended to use Zowe Explorer, with which you can edit COBOL, PL/I, and HLASM files that are opened on z/OS MVS™ and z/OS UNIX System Services, and run JCL and browse job spool files.

To connect, see:

- [Connecting to z/OS with Zowe Explorer walk through](https://ibm.github.io/zopeneditor-about/Docs/connect_to_zos_with_zowe_explorer_e2e.html#overview).
- [Connecting to z/OS using Zowe CLI walk through](https://ibm.github.io/zopeneditor-about/Docs/connect_to_zos_with_zowe_cli_e2e.html#creating-a-zowe-team-configuration-file)


When you have the Zowe Explorer VS Code extension [installed](https://docs.zowe.org/stable/user-guide/install-overview), you can open the following three views by clicking the Zowe icon on the VS Code Activity bar to interact with z/OS® resources:

- **DATA SETS** view that shows your data sets and members and allows you to directly open, edit, and save your programs against MVS™.
- **UNIX SYSTEM SERVICES (USS)** view that shows you USS folders and files that you can also directly open, edit, and save.
- **JOBS** view that gives you access to your jobs and spool files.

See the [documentation in the VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=Zowe.vscode-extension-for-zowe) for details on using and configuring each view. More examples are available in the section [How to manipulate data sets with Zowe Explorer and Submitting JCL to compile, link, and run jobs](https://ibm.github.io/zopeneditor-about/Docs/interact_zos_zowe_explorer.html#example-how-to-manipulate-data-sets-with-zowe-explorer) sections.


## IBM Z Open Editor

[IBM Z Open Editor](https://ibm.github.io/zopeneditor-about/) is for developers interested in Z enterprise application development, especially those who prefer a modern development environment. By bringing IBM z/OS language support to one of today’s most popular code editors, Visual Studio Code (VS Code), IBM Z Open Editor gives developers the freedom to code in COBOL, PL/I, High-Level Assembler, or REXX using the same editor they can use for languages such as Java and JavaScript. 

IBM Z Open Editor is a FREE [downloadable extension](https://ibm.github.io/zopeneditor-about/Docs/getting_started.html#installing-the-ibm-z-open-editor-vs-code-extension) in Visual Studio Code’s marketplace.

See [IBM Z Open Editor](https://ibm.github.io/zopeneditor-about/Docs/introduction.html#key-capabilities) on GitHub.

For tutorials on using the Z Open Editor, see [Tutorial overview](https://ibm.github.io/zopeneditor-about/Docs/tutorial_overview.html).

To get started, see [Getting started with IBM Z Open Editor](https://ibm.github.io/zopeneditor-about/Docs/getting_started.html#privacy-notice).

## IBM Z Open Debug

**IBM Z Open Debug** is a Visual Studio Code extension that brings COBOL and PL/I applications debugging support to VS Code. It provides developers a modern debugging experience for IBM Z Enterprise Languages. 

To debug your code, you will:

- [Prepare your application environment](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=applications-preparing-your-application-environment)
- [Prepare your program for debugging](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=applications-preparing-your-program-debugging)
- [Manage debug profiles](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=da-managing-debug-profiles-z-open-debug-profiles-view)
- [Launch and debug your applications](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=applications-launching-debugging-your-application)

See [Setting up for IBM Z Open Debug](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=code-setting-up-z-open-debug).

## Visual Studio Code Tutorials for Z

There are several tutorials available to learn about using Visual Studio Code with Z. See [Tutorial overview](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=code-tutorial).

If you are ready to get hands-on with IBM Z® Open Editor, you can use the [sample repository of COBOL, PL/I, HLASM, and REXX files](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/samplefiles.html) to walk through the tutorials and explore the features of IBM Z Open Editor.

Once you have the sample files, you can start by making code changes to:

- [COBOL](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/tutorial_cobol.html)
- [HLASM](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/tutorial_assembler.html)
- [REXX](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/tutorial_rexx.html) programs to learn about the editing capabilities.

After you complete code changes on your machine, you might want to go ahead and manage z/OS® resources. To learn more about how to interact with z/OS using IBM Z Open Editor and its integrations, refer to the following tutorials:

- [Managing z/OS resources with IBM® RSE API Plug-in for Zowe™ CLI tutorial](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/rse_tutorial.html). Provides examples on how to use Zowe Explorer, IBM RSE API Plug-in for Zowe CLI commands, and a script to interact with z/OS. This tutorial is relevant when RSE API is installed and configured on the host.
- [Submitting JCL to compile, link, and run jobs tutorial](https://www.ibm.com/docs/en/SSQ2R2_16.0.0/com.ibm.wazi.developer.vscode.doc/zowe_submitjcl.html). Provides examples on how to use Zowe CLI commands and Zowe Explorer to submit JCL.

## Installation

See:

- [Installing Wazi for VS Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=iwvc-installing-wazi-vs-code).
- [Configuring Wazi for VS Code](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=code-configuring-wazi-vs)

## Your Learning course

[Cloud native development with IBM Z and Cloud Modernization Stack Fundamentals](https://yourlearning.ibm.com/credential/CREDLY-5bf19885-2196-4b0c-81af-5013c9343e6a) provides has a good understanding of the capabilities, benefits and usage of Cloud native development with IBM Z and Cloud Modernization Stack. This includes capabilities and benefits of Cloud native development with IBM Z and Cloud Modernization Stack, how to use IBM Wazi, and how it supports J2C.  

## References

- [Developing with IBM Wazi Developer for VS Code](https://www.ibm.com/docs/en/wdfrhcw/1.4.0?topic=ide-option-2-developing-vs-code)
- [Developing applications with Wazi Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=wazi-developing-applications-code)