# Wazi Code

Choose one of these IDEs to connect to a z/OS system and edit, build, and debug mainframe applications.

**IBM Wazi Code** is a productive development environment that fully integrates into any enterprise-wide standard DevOps pipeline. 

The **Code** component of IBM Wazi Developer for Red Hat CodeReady Workspaces enables the development of COBOL, PL/I, High-Level Assembler (HLASM), REXX programs through the use of an industry-standard integrated development environment (IDE). 

The Code component of IBM Wazi enables the development of COBOL, PL/I, High-Level Assembler (HLASM), REXX programs through the use of an industry-standard integrated development environment (IDE). The Code component offers essential developer capabilities that include edit, build, and debug across different IDE options. 

You can also get the interactive access to z/OS systems with the Code component. It also integrates with modern SCMs, for example, Git. By using the Code component, developers unfamiliar with z/OS and IBM Z mainframe can get up to speed quickly and become productive in developing and delivering applications.

These IDE options are available to you:

- Red Hat OpenShift Dev Spaces, realized by IBM Wazi for Dev Spaces
- Microsoft VS Code, realized by IBM Wazi for VS Code

## Features

- Modern editors for COBOL, PL/I, JCL, HLASM, and REXX that provide language-specific features such as syntax highlighting, outline view, declaration hovering, code completion, snippets, copybook preview, copybook navigation, and basic refactoring.
- Source code management (SCM) integration to enable integration with any flavor of Git, a popular and modern parallel development SCM.
- Intelligent build capability that enables developers to perform a user build with IBM Dependency Based Build for any flavor of Git.
- An integrated debugger to facilitate COBOL, PL/I, and HLASM debugging through IBM z/OS Debugger.
- Integrations that enable developers to work with z/OS resources such as MVS™ and UNIX files and JES jobs.

## Select IDE

As the first step, you should plan and decide which IDE client you want to use to gain development support for z/OS applications.

For more information, see [Developing applications with Wazi Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=wazi-developing-applications-code).

!!! info

    Wazi for Dev Spaces can support almost all the capabilities that are available in Wazi for VS Code in the OpenShift cloud environment, with some differences on user experience.

    For a deep dive into the similarities and differences in the two enviornments, see [Why do instructions for Wazi for VS Code also apply to Wazi for Dev Spaces?](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-choosing-ide-client#choosing-an-ide__explanation__title__1)

### Wazi for VS Code

Runs on desktop. It provides a set of Microsoft VS Code extensions to extend VS Code to deliver a simple and familiar edit, build, and debug experience.

VS Code is a popular desktop editor among many current and next generation developers. IBM Enterprise language support in VS Code makes enterprise programming more attractive and productive by allowing developers to use this popular editor, with the option to integrate numerous other extensions from the VS Code Marketplace.

See [Developing with IBM Wazi for VS Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-option-1-developing-wazi-vs).

### Wazi for Dev Spaces

With this in-browser IDE, you can code, build, test, debug, and run applications from any machine without any local environment configurations. Upon a single-click, team members can get their own workspace up and running.

Wazi for Dev Spaces supports almost all the capabilities that are available in Wazi for VS Code in the OpenShift cloud environment, with some differences on user experience. 

You can run a _user build_ to compile and link programs during coding and unit testing before the code is ready to be exposed to the repository for others to use. With user build, you can compile your program without having to perform commits or pushes. With the user build setting enabled in your IDE, you can trigger user build simply by right-clicking inside a COBOL, PL/I, or HLASM file. Refer to the full [IBM User Build documentation](https://www.ibm.com/docs/en/SSV97FN_2022.1.1/wazidoc/com.ibm.wazi.developer.vscode.doc/setting_user_build.html) to learn more about how to leverage user build.

See [Developing with IBM Wazi for Dev Spaces](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-option-2-developing-wazi-dev-spaces).

## Checklists

All the IDE options provided by IBM Wazi are built on the client/server architecture:

- The client side provides the user interface that communicates with the server.
- The server side is a set of z/OS host components.

For checklists in setting up your dev environment on developer computers and hosts, see [Checklists](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-checklists).



## References

- [Developing applications with Wazi Code](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=wazi-developing-applications-code)
- [Choosing an IDE client](https://www.ibm.com/docs/en/cloud-paks/z-modernization-stack/2023.4?topic=code-choosing-ide-client).
- [End-to-end workflow](https://www.ibm.com/docs/en/wdfrhcw/1.4.0?topic=overview-end-end-workflow)
