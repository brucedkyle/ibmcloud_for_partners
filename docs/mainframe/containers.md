# Containers on Z with LinuxONE and OpenShift

With IBM Z integrated into a hybrid cloud platform that is based on [Red Hat® OpenShift®](https://cloud.redhat.com/blog/ibm-and-red-hat-bring-openshift-to-ibm-z-and-linuxone?_ga=2.24696698.1599634280.1696544389-1455186305.1696267056&_gl=1*bz1d0m*_ga*MTQ1NTE4NjMwNS4xNjk2MjY3MDU2*_ga_FYECCCS21D*MTY5NjYxNDc5OC4zNi4xLjE2OTY2MTcxOTAuMC4wLjA.), businesses can use the resiliency, security, scale, and data gravity of IBM Z to gain greater infrastructure efficiency and lower compliance costs.

## LinuxONE

IBM LinuxONE is an enterprise-grade Linux® server that brings together IBM’s experience in building Z mainframe systems with the openness of the Linux operating system.

With a unique architecture designed to meet the needs of mission-critical workloads, LinuxONE provides a sustainable, secure and scalable system for companies of all sizes. 

## Benefits of containized workloads

The primary advantage of containers, especially as compared to a VM, is that they provide a level of abstraction that makes them lightweight and portable. Their primary benefits include:

**Lightweight**: Containers share the machine OS kernel, eliminating the need for a full OS instance per application and making container files small and easy on resources. Their smaller size, especially compared to VMs, means containers can spin up quickly and better support [cloud-native](https://www.ibm.com/topics/cloud-native?_ga=2.63447084.220443453.1680552572-1232242216.1680552572) applications that scale horizontally.

**Portable and platform-independent**: Containers carry all their dependencies with them, meaning that software can be written once and then run without needing to be re-configured across laptops, cloud and on-premises computing environments.

**Supports modern development and architecture**: Due to a combination of their deployment portability/consistency across platforms and their small size, containers are an ideal fit for modern development and application patterns—such as DevOps, serverless and microservices—that are built using regular code deployments in small increments.

**Improves utilization**: Like VMs before them, containers enable developers and operators to improve CPU and memory utilization of physical machines. Where containers go even further is that because they also enable microservices architecture, application components can be deployed and scaled more granularly—an attractive alternative to having to scale up an entire monolithic application because a single component is struggling with its load.

In a recent [IBM survey](https://www.ibm.com/downloads/cas/VG8KRPRM?_ga=2.100147485.220443453.1680552572-1232242216.1680552572), developers and IT executives reported many other benefits of using containers.

## Tutorial

Learn how to launch a simple NGINX web server container from a Dockerfile using the OpenShift Container Platform on the LinuxONE Community Cloud.

See [Use the Red Hat OpenShift Container Platform on the IBM LinuxONE Community Cloud to launch a web server](https://developer.ibm.com/tutorials/red-hat-openshift-container-platform-linuxone-community-cloud-web-server/)

## References

- [IBM and Red Hat bring OpenShift to IBM Z and LinuxONE](https://cloud.redhat.com/blog/ibm-and-red-hat-bring-openshift-to-ibm-z-and-linuxone)