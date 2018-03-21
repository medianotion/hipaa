# HIPAA Cloudformation template
This is a modification of the AWS HIPAA template found here:  https://aws.amazon.com/quickstart/architecture/accelerator-hipaa/

The customizations are:

1.  Setting an S3 location for the SSL certificates.  The original template generated temp SSL certs and installed them on the proxy and app instances.  This template allows the user to specify their SSL certs in an S3 location and the template installs them on the proxy and app instances.
2.  Allows for the user to choose the database engine.
3.  Uses NAT Gatways by default instead of NAT instances.
4.  Does not install wordpress on the app instances.
5.  Installs CodeDeploy on the app instances.
