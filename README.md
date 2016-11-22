# IBM Application Security on Cloud Bamboo Plug-in

Easily integrate security scanning with the [IBM Application Security on Cloud](https://appscan.ibmcloud.com) service into your builds running on Atlassian Bamboo.

# Prerequisites

- An account on the [IBM Application Security on Cloud](https://appscan.ibmcloud.com) service.
- The plug-in has been tested to run on Bamboo server version 5.13.2 or later.
- To build the plug-in, you will need to install the [Atlassian pluign SDK](https://developer.atlassian.com/docs/getting-started).
- You will need to setup the Static Analyzer Client Utility on your Bamboo server (to initiate scans on local agents), or on remote agent machines. For more information on obtaining the client utility, see the docs [here](http://www.ibm.com/support/knowledgecenter/SSYJJF_1.0.0/ApplicationSecurityonCloud/src_scanning.html).

# Building the Plug-in

- Navigate to the plug-in's root folder and issue the `atlas-package` command. The built plug-in JAR will be in the target folder.

# Installation and Configuration

1. Install the plug-in via the Bamboo's administration dashboard. After installing the plug-in, it will appear in the list of user installed add-ons.

   ![](https://github.com/AppSecDev/asoc-bamboo-plugin/blob/master/images/install1.png)

2. Via Bamboo's administration dashboard, add the SA Client capability to your server (for local agents), or to your remote agents. Specify the path to the Static Analyzer Client Utility.

   ![](https://github.com/AppSecDev/asoc-bamboo-plugin/blob/master/images/install2.png)

3. Enter your IBM Application Security on Cloud account username and password in Bamboo's shared credentials page.

# Adding the SAST Scan Task to your Build Plan

1. Add the SAST scan task to your build plan after your artifacts have been built.

# License

All files found in this project are licensed under the [Apache License 2.0](LICENSE).

