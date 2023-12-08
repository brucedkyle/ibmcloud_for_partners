# API for Z

An [API-centric](https://www.ibm.com/topics/api) integration strategy is fundamental to mainframe application modernization. New cloud-native channel applications need access to mainframe applications and data, which hosts core business logic for many industries. The core mainframe applications like COBOL, CICS and IMS can be [exposed](https://www.ibm.com/cloud/architecture/architectures/z-expose-apis-pattern) through APIs. 

!!! info "Client challenges"

    - How to access core assets (Apps/Data) on mainframe
    - How to modernize legacy mainframe applications
    - How to respond to events both from mainframe as well as from cloud centric events
    - Exposing functionality to 3rd party Enterprise Organizations
    - Transforming complex monolithic core applications to microservices

## Benefits of API development for mainframe on IBM Cloud

- Enterprise mainframe application modernization with z Mod Stack and Wazi as a Service.
- Identification of security vulnerabilities during DevOps/API creation
- Best secure platform for API development and invocation
- z/OS VSI (Wazi) is 15x faster than emulated x86
- Secure API Management with z-Connect and IBM Cloud API Connect services
- Secure Network Isolation with Red Hat OpenShift Kubernetes on IBM Cloud (ROKS) and Virtual Server Instance (VSI) patterns on IBM Cloud framework for Financial Services
- Secure cloud services like HPCS, SCC

This article provides concrete steps you can make to satisfy the client challenges:

- Secure landing zone
- DevOps pipeline

## Secure Landing Zone

IBM Cloud offers a [secure framework to manage the lifecycle of mainframe APIs](https://github.com/terraform-ibm-modules/terraform-ibm-landing-zone-vsi) for development and test through hybrid cloud. This is supported by the [IBM Z and Cloud Modernization Stack](https://www.ibm.com/products/z-and-cloud-modernization-stack) running on IBM Cloud.

The following diagram shows virtual server instances (VSI) across multiple subnets with any number of block storage volumes that are connected by any number of load balancers.

![vsi-lb](./media/vsi-lb.png)

For more information, see [IBM Secure Landing Zone VSI Module](https://github.com/terraform-ibm-modules/terraform-ibm-landing-zone-vsi).

For more information on VPCs, see [IBM Cloud VPC Solutions](../cloud/vpc.md).

See [Accelerate application modernization and IT automation with IBM Z and Cloud Modernization Stack](https://www.ibm.com/downloads/cas/A8DQ61MR) briefing.

## DevOps pipeline

With a high-performing z/OS VSI provisioned in IBM Cloud VPC and integrated with [CI/CD pipelines](https://www.ibm.com/cloud/blog/ci-cd-pipeline), IBM Cloud can provide a secure development and test environment to create new IBM Z-centric APIs, and it can use IBM Cloud for Financial Services features like the [IBM Cloud Security and Compliance Center](https://www.ibm.com/cloud/security-and-compliance-center) to validate the compliance requirements.

For more step-by-step guidance on setting up a DevOps pipeline for mainframe, see [A modern DevOps platform for mainframe applications with IBM Cloud](./devops.md).

## Development of APIs

As modern systems interact with each other through REST APIs, mainframe applications and data 
can also be exposed and extended through REST APIs. IBM zSystems has developed a set of tools
to help create, expose and even consume the APIs. One of the key tools available for this is IBM® 
z/OS® Connect EE which can facilitate the creation of APIs to expose mainframe applications and 
data. It can also consume external APIs to extend and modernize existing mainframe applications.

## Architecture

The integration of IBM zSystem centric assets with cloud native distributed applications can be 
classified into three pattern types from an architecture point of view. These are 

- Application centric integration patterns
- Data centric integration patterns
- Event centric integration patterns

This reference solution architecture described here implements application centric pattern using IBM 
Cloud and follows principles of [IBM zSystem design patterns](https://developer.ibm.com/components/zos/patterns/).

### Application centric integration pattern

Application centric integration patterns and event centric integration patterns can be further classified into five subcategories shown below, solely based on the techniques used to modernize mainframe applications:

1. **Expose pattern**. With this pattern, core mainframe assets can be exposed as APIs and other enterprise applications running either on-premises or on cloud can invoke these APIs to easily build powerful hybrid cloud applications
2. **Extend pattern**. With this pattern, core mainframe applications can be modernized with 
additional features by consuming other enterprise applications including cloud-based services provided by other organizations made available as APIs
3. **Enhance pattern**. With this pattern, it is possible to selectively enhance a sub-part of a bigger core mainframe monolithic application like presentation layer, shared function, business rules etc., which will address the immediate business needs without embarking on a risky total 
rewrite of core applications
4. **Respond in real-time pattern**. This is part of an event centric pattern, where other enterprise applications integrated with core mainframe applications can respond in real time to events occurring in mainframe assets
5. **Respond to external events pattern**. Core mainframe applications can run certain tasks
responding to other enterprise application events through event-based model 

This reference architecture describes application centric pattern and help guide enterprise developers to securely integrate cloud native applications with core mainframe applications through unique development and test features available in IBM Cloud.

## Next steps

See:

- [Expose through APIs pattern](https://www.ibm.com/cloud/architecture/architectures/z-expose-apis-pattern). Access mainframe applications and data by using standards-based REST APIs with IBM® z/OS® Connect EE. Manage APIs by using industry-standard API management solutions, including solutions by IBM.
- [Accelerate application modernization and IT automation with IBM Z and Cloud Modernization Stack](https://www.ibm.com/downloads/cas/A8DQ61MR)
- Redbooks [Hybrid Cloud with IBM Z Redbook](https://www.redbooks.ibm.com/abstracts/sg248532.html)


## Reference

- [Mainframe Application Modernization with IBM Cloud and IBM zSystems](https://www.ibm.com/blog/mainframe-application-modernization-with-ibm-cloud-and-ibm-zsystems/)
- [IBM Z and Cloud Modernization Stack](https://www.ibm.com/products/z-and-cloud-modernization-stack), a hybrid approach combining the best of the cloud with IBM zSystems.
- [Simplify access to mainframe applications with API Strategy](https://www.ibm.com/downloads/cas/EX4O1LJY)

## Credits

- Surya V Duggirala, IBM Cloud Platform Engineering Guild Leader
- Pradeep Kadiyala, Senior Solutions Architect for IBM Cloud Financial Services