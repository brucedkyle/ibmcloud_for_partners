# Wazi Deploy

**IBM® Wazi Deploy** accelerates the customization and automation of z/OS® application deployment for test and production environments in a continuous integration/continuous delivery (CI/CD) pipeline. New versions of applications can be deployed as frequently as necessary, without stopping the application server, as the applications are deployed in real time. It uses the open source standard technologies and languages that are widely used with distributed and Cloud applications.

## How to use Wazi Deploy

No server is involved. Wazi Deploy is solely constituted of a command-line interface.

Wazi Deploy can be easily integrated into a continuous integration/continuous delivery (CI/CD) pipeline, which is constituted of the following two parts:

- The continuous integration, where the applications are built. The builds can be triggered after code fixes or the development of new features. The build results, such as load modules or DBRMs, are uploaded to an artifact repository.
- The continuous delivery, where Wazi Deploy is triggered. Wazi Deploy deploys the binary files that have been produced and uploaded to an artifact repository. It deploys the artifacts to a test environment, and if the tests are correct, to the integration and production environment. So the same deployment process applies from test to production.

The same end-to-end pipeline can be used across the organization for z/OS, distributed, and Cloud applications. You can watch the Wazi Deploy video to see how Wazi Deploy is used in a CI/CD pipeline to automate the deployment of z/OS applications.

The traceability of the deployed artifacts is covered by the production of evidence files at the end of each deployment step.

For this release, Wazi Deploy is designed to deploy CICS® Db2®, IMS, and batch applications only.

For more details, see [Deploying to z/OS with IBM Wazi Deploy](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=deploying-zos-wazi-deploy).

## References

- [Deploying to z/OS with IBM Wazi Deploy](https://www.ibm.com/docs/en/developer-for-zos/16.0?topic=deploying-zos-wazi-deploy)