## Getting started with IBM Wazi as a Service

Learn how to develop and test your applications with your virtual server instance by using IBM's development tools portfolio.

You can learn how to use tools such as VS Code and Eclipse, understand Cloud concepts and tools and how they add value to z/OS DevOps.

You can also learn new technologies such as Ansible for automation, DBB and Groovy for build, GitLab and Tekton for serverless pipelines.

The tutorial contains the following topics:

- Checklist for the prerequisites
- How to configure access to the available services in the VSI
- How to develop and test with IBM Wazi for VS Code
- How to develop and test with IBM Wazi for Eclipse or IBM Developer for z/OS
- How to deploy and use IBM Wazi for Dev Spaces from a Red Hat OpenShift cluster in IBM Cloud VPC

See [Getting started with IBM Wazi as a Service](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=getting-started-wazi-as-service).

## Wazi journey

The following illustration shows Wazi as a Service journey map.

[![journey map](./media/journey-map.svg)](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=use-cases)

To get started rapidly, start from selecting one of the following use cases and perform the required tasks.

Choose:

- z/OS image

    - Virtualized z/OS using standard images
    - Virtualized z/OS using custom images

- Choose Wazi Code development environment:

    - Web based Wazi Development (Dev Spaces)
    - VS Code on desktop
    - Eclipse on desktop

Those choices will dictate your required tasks.

| Standard or custom image | Wazi Code dev enviornment | Tasks |
| -- | -- | -- |
| Standard virtualized z/OS | Wazi for VS Code | [Use case](#standard-virtualized-zos-with-ibm-wazi-for-vs-code) |
| Standard virtualized z/OS | Wazi for Eclipse | [Use case](#standard-virtualized-zos-with-ibm-wazi-for-eclipse) |
| Standard virtualized z/OS | Web-based IBM Wazi | [Use case](#standard-virtualized-zos-with-web-based-ibm-wazi) |
| Customized and virtualized z/OS | Wazi for VS Code | [Use case](#customized-and-virtualized-zos-with-ibm-wazi-for-vs-code) |
| Customized and virtualized z/OS | Wazi for Eclipse | [Use case](#customized-and-virtualized-zos-with-ibm-wazi-for-eclipse) |
| Customized and virtualized z/OS | Web-based IBM Wazi | [Use case](#customized-and-virtualized-zos-with-web-based-ibm-wazi) |


### Standard virtualized z/OS with IBM Wazi for VS Code

1. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with a standard z/OS dev & test stock image to initiate your z/OS environment.
2. **Develop and test with IBM Wazi for VS Code**. On your desktop, set up the VS Code extensions of IBM Wazi for VS Code, and connect to the z/OS VSI to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-1.html).

Next, learn [Developing and testing with IBM Wazi for VS Code](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=service-developing-testing-wazi-vs-code) for:

- How to connect IBM Z Open Editor with Zowe Explorer in VS Code.
- Run dependency-based user builds from Z Open Editor
- Run debug session from Z Open Editor

### Standard virtualized z/OS with IBM Wazi for Eclipse

1. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with standard z/OS dev & test stock image to initiate your z/OS environment.
2. **Develop and test with IBM Wazi for Eclipse**. On your desktop, set up IBM Wazi for Eclipse, and connect to the sandbox instance to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-2.html).

Next, learn [Developing and testing with IBM Wazi for Eclipse or IBM Developer for z/OS](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=service-developing-testing-wazi-eclipse-developer-zos) to:

- Connect IBM Wazi for Eclipse to IBM Developer for z/OS.
- Run dependency-based user builds for IBM Wazi for Eclipse.
- Run a debug session from IBM Wazi for Eclipse.

### Standard virtualized z/OS with web-based IBM Wazi

1. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with standard z/OS dev & test stock image to initiate your z/OS environment.
2. **Develop and test with IBM Wazi for Dev Spaces**. In Red Hat OpenShift, create a development workspace and connect to the z/OS VSI to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-3.html).

Next learn [Deploying and using IBM Wazi for Dev Spaces from a Red Hat OpenShift cluster in your VPC](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=gswas-deploying-using-wazi-dev-spaces-from-red-hat-openshift-cluster-in-your-vpc) to:

- Create Red Hat OpenShift cluster
- Deploy and configure IBM Wazi for DevSpaces
- Create a development workspace

### Customized and virtualized z/OS with IBM Wazi for VS Code

1. **Create a custom z/OS image with IBM Wazi Image Builder**. Bring your own z/OS image with customized z/OS components and data sets, and deploy the image to IBM Cloud.
2. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with deployed z/OS custom image to initiate your z/OS environment.
3. **Develop and test with IBM Wazi for VS Code**. On your desktop, set up the VS Code extensions of IBM Wazi for VS Code, and connect to the z/OS VSI to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-4.html).

Next, learn [Developing and testing with IBM Wazi for VS Code](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=service-developing-testing-wazi-vs-code) for:

- How to connect IBM Z Open Editor with Zowe Explorer in VS Code.
- Run dependency-based user builds from Z Open Editor
- Run debug session from Z Open Editor

### Customized and virtualized z/OS with IBM Wazi for Eclipse

1. **Create a custom z/OS image with IBM Wazi Image Builder**. Bring your own z/OS image with customized z/OS components and data sets, and deploy the image to IBM Cloud.
2. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with deployed z/OS custom image to initiate your z/OS environment.
3. **Develop and test with IBM Wazi for Eclipse**. On your desktop, set up IBM Wazi for Eclipse, and connect to the sandbox instance to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-5.html).

Next, learn [Developing and testing with IBM Wazi for Eclipse or IBM Developer for z/OS](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=service-developing-testing-wazi-eclipse-developer-zos) to:

- Connect IBM Wazi for Eclipse to IBM Developer for z/OS.
- Run dependency-based user builds for IBM Wazi for Eclipse.
- Run a debug session from IBM Wazi for Eclipse.

### Customized and virtualized z/OS with web-based IBM Wazi

1. **Create a custom z/OS image with IBM Wazi Image Builder**. Bring your own z/OS image with customized z/OS components and data sets, and deploy the image to IBM Cloud.
2. **Create a z/OS VSI in IBM Cloud VPC**. In IBM Cloud, create a z/OS VSI with deployed z/OS custom image to initiate your z/OS environment.
3. **Develop and test with IBM Wazi for Dev Spaces**. In Red Hat OpenShift, create a development workspace and connect to the z/OS VSI to debug, code, and build your applications.

To adopt this use case, follow the [required tasks](https://www.ibm.com/docs/en/SSSTT9_1.0.0/wazi-aas-use-case-6.html).

Next learn [Deploying and using IBM Wazi for Dev Spaces from a Red Hat OpenShift cluster in your VPC](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=gswas-deploying-using-wazi-dev-spaces-from-red-hat-openshift-cluster-in-your-vpc) to:

- Create Red Hat OpenShift cluster
- Deploy and configure IBM Wazi for DevSpaces
- Create a development workspace

## References

- Product page [IBM Wazi as a Service](https://www.ibm.com/cloud/wazi-as-a-service)
- [Getting started with IBM Wazi as a Service](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=getting-started-wazi-as-service)
- Wazi as a Service [Use cases](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=use-cases)