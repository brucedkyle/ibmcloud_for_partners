# Bring-your-own-image using Wazi Image Builder

**IBM® Wazi Image Builder** enables enterprises to extract your on-premise IBM Z® platforms and deploy it as a custom image through API or web-based graphical interface for use within the IBM Cloud® Virtual Private Cloud (VPC) infrastructure. Wazi Image Builder can be installed on an x86_64 Linux® system hosted either in a cloud or an on-premise physical or virtual machine.

Wazi Image Builder provides the following features:

- An application development and testing environment that can improve development infrastructure availability and flexibility.
- Current levels of IBM z/OS® software that give access to new runtime capabilities for development and testing for enterprises.
- Mixed workload support for enterprises, which can help reduce the development costs.
- An approachable and portable environment for education on Z for enterprises.
- A web-based interface to extract, manage, and deploy the images from existing Z packages.
- Creating and managing images from various sources.
- Deploying images for developers and testers in a self-service automated way.
- Monitoring the status and availability of all created assets and target environments.

## Source environments

Wazi Image Builder can work with your source environments to extract and deploy the necessary volumes to target environments. The following source environment types are supported:

- **Genuine z/OS on IBM Z**. ZD&T z/OS Extraction Utilities must be installed and configured on such a source environment to extract z/OS artifacts.
- **Existing z/OS instances**. ZD&T z/OS Extraction Utilities must be installed and configured on such a source environment to extract z/OS artifacts.

You can specify and configure source environments on the web server. For more information, see [Adding source environments](https://www.ibm.com/docs/en/SSSTT9_1.0.0/com.ibm.zsys.rdt.tools.user.guide.doc/topics/config_source.html).

## Flow using Image Builder

The following diagram show the content flow connecting up IBM Cloud with IBM Wazi Image Builder.

![image builder](./media/flow-final.png)

## Next steps

See [Bringing your own image with Wazi Image Builder](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=bringing-your-own-image-wazi-image-builder) product documentation for:

- Prerequisites and installation
- Setting up networking for on-premises z/OS environments
- Creating, monitoring, and managing components
- Creating, monitoring, and managing z/OS images
- Deploying images to Wazi target environment

See [Cloud Native IBM Z DevOps as a Service](https://mediacenter.ibm.com/playlist/details/1_5q5qeehb/) videos.

## References

- [Bringing your own image with Wazi Image Builder](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=bringing-your-own-image-wazi-image-builder)