# DevTest on mainframe in IBM Cloud

You can now spin up a built-for-a-purpose z/OS dev and test virtual server in six minutes or less[^1]. You can either use a pre-installed stock image or extract components from an on-prem system and deploy a custom image onto the virtual server using IBM Wazi Image Builder in IBM Cloud’s Virtual Private Cloud environment. This environment is a logically isolated, highly secured private space running in IBM Cloud, thereby eliminating the wait times involved in getting access to resources.

**IBM Wazi as a Service (IBM Wazi aaS)** offers self-serve access to z/OS systems and shorten your development and testing cycles. You can further integrate a secure toolchain for continuous delivery to enhance your developer productivity. With increased efficiency in code development and testing, you can reduce time to market.

!!! quote

    [IBM Wazi aaS](https://www.ibm.com/cloud/wazi-as-a-service) provides us with the much-needed agility to our development process. Within minutes, developers can now setup their own custom z/OS environment, use automation and work in total isolation without any dependency. This marks a huge shift in how we can deliver services to our customers &dash; _Harry Mavrakis, Chief Enterprise Architect from Eurobank_.

IBM Wazi aaS enables you to have self-serve access to z/OS systems and shorten your development and testing cycles. You can further integrate a secure toolchain for continuous delivery to enhance your developer productivity. With increased efficiency in code development and testing, you can reduce time to market.

!!! key "Challenges"

    Number one challenge to using mainframes is now lack of resources and skills - high costs moved to the very bottom of the list. &dash; _IBM IBV 2023 Mainframe executive pulse survey_

    Executives are now looking for more value from mainframe – some of these are new sources of value such as resilience, optimization and regulatory compliance. 

## Continuous test environment

You can now _Shift Left_ and implement a continuous-testing process, bringing real-time feedback into the development cycle. Isolated development environments — combined with _DevSecOps testing tools_ — enable your developers to start testing at a much earlier stage of the development lifecyle on a z/OS dev and test virtual server. The virtual server running on real zSystems hardware provides up to 15x better performance than comparable x86 offerings[^2]. This virtual server enables you to accelerate software release cycles and improve software quality.

## Continous delivery

Your developers can now experiment with enterprise-ready _DevSecOps_ using IBM Cloud Continuous Delivery. This service allows you to provision an integrated secure toolchain using customizable, shareable templates with tools from IBM, third parties and open source. You can further automate the delivery pipeline, manage source code and track work with Git repositories and issue tracking hosted by IBM and built on GitLab Community Edition. This can reduce barriers to entry for developers and open the possibility of improving developer efficiency.

## Next steps

- Visit the [IBM Wazi as a Service](https://www.ibm.com/cloud/wazi-as-a-service) page
- Watch [demos](https://mediacenter.ibm.com/playlist/dedicated/189147203/1_5q5qeehb/1_9agz7ap1) of IBM Wazi as a Service
- Read the IBM Wazi as a Service [technical documentation](https://www.ibm.com/docs/en/wazi-aas/1.0.0)

See [IBM Wazi as a Service overview](./wazi.md) in this wiki.

## References

- [Introducing IBM Wazi as a Service to Accelerate Innovation with IBM z/OS Dev and Test](https://www.ibm.com/blog/announcement/introducing-ibm-wazi-as-a-service/)

### IBM Partners

- [Accelerate application modernization with IBM Z and Cloud](https://ibm.seismic.com/Link/Content/DCR4jCd9G2J348M2HV38mccjFpBB)
- See IBM Institute for Business Value paper [Application modernization on the mainframe](https://www.ibm.com/thought-leadership/institute-business-value/report/application-modernization-mainframe)

[^1]: 
    On average, creating an experimental IBM Cloud z/OS Virtual Server Instance (VSI) of a z/OS 2.4 stock image and a mz2o-2×16 VSI profile takes 1 minute, and it is ready for user login (SSH) in 5.5 minutes. Disclaimer: Measurements were done across two different IBM Cloud production sites using an experimental version of z/OS 2.4 stock image and a mz2o-2×16 VSI profile. Measurements were performed with Ansible automation based on the examples here. Results may vary.
[^2]:
    Applications compile faster on an experimental IBM Cloud z/OS Virtual Server Instance (VSI) than on IBM Z Development and Test (ZD&T) EE V13.3 running on the compared IBM Cloud x86 VSI — about 15x faster compilation of Java applications, about 12x faster compilation of C applications and about 8x faster batch compilations of COBOL/FORTRAN applications. Disclaimer: Performance results based on IBM internal tests running application compiles on an experimental IBM Cloud z/OS V2R4 Virtual Server Instance (VSI) with profile mz2o-2×16 versus on IBM ZD&T EE V13.3 running in an IBM Cloud x86 VSI with profile mx2-2×16. IBM ZD&T was running on Ubuntu 20.4 on a x86 Production VSI with a Cascade Lake Intel Xeon Platinum CPU @ 2.4GHz. Both z/OS VSI and ZD&T were configured with 2 vCPUs, 16GB memory, and 1 TB Block storage with 10 IOPS/GB. The following applications were compiled — a Java application that processes SMF records, a C application that processes IBM Z hardware diagnostic data, a COBOL application that creates and updates records on a file and a FORTRAN statistical application. Results may vary.