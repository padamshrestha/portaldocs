## Introduction

If you are working on an Azure service and want to expose UI to your customers in the Azure portal then this is the right starting point. The portal has an extension model where each team that builds UI creates and deploys an extension. This process requires a relationship to be established between your team and the central portal team. This document walks you through the process of onboarding your team and starting that relationship. 
   
## Step by Step Process overview

Onboarding a service, or developing a Portal extension, has three phases: onboarding, development, and deployment. The process is specified in the following image.

![alt-text](../media/portalfx-extensions-onboarding/azure-onboarding.png "Azure Onboarding Process")

# Phase 1 - Onboarding

## Kickoff Meeting
 
There are lots of docs here. We recommend you send mail to <a href="mailto:ibiza-onboarding-kick@microsoft.com?subject=Kickoff Meeting Request&body=My team would like to meet with you to learn about the Azure onboarding process.">ibiza-onboarding-kick@microsoft.com</a> and request a kickoff meeting. Someone from our team will spend 30 minutes walking through the process at a high level. We can point you in the right direction regarding the latest patterns and practices. We can also answer any questions you have. Finally, we can talk about how the relationship between our teams is managed.

## Join DLs and request permissions

Request the following permissions to stay current on product roadmaps, get news on latest features, and read workshop announcements.

* PMs and Developer Leads need to join the `ibizapartners PM`  group by clicking on this link: [http://igroup/join/ibizapartners-pm](http://igroup/join/ibizapartners-pm). 

* Developers should join the  `ibizapartners DEV` group by clicking on this  link:  [http://igroup/join/ibizapartners-dev](http://igroup/join/ibizapartners-dev). 

* Developers should join the appropriate group listed on [http://aka.ms/standardaccess](http://aka.ms/standardaccess) to get access to portal telemetry. All groups on this page receive access. 

* Developers should join the  `Azure Portal Core Team - 15003(15003)` group by using this link: [http://ramweb](http://ramweb).

* PMs, Developers, and Developer Leads should subscribe to the partner request process by joining the ```Uservoice ``` group at this link:  [https://aka.ms/portalfx/uservoice](https://aka.ms/portalfx/uservoice). For more information about the partner request process, see [portalfx-extension-partner-request-process.md](portalfx-extension-partner-request-process.md).

* PMs, Developers, and Developer Leads should receive notifications on breaking changes by joining the ```ibizabreak ``` group at  this  link:  [http://igroup/join/ibizabreak](http://igroup/join/ibizabreak).

* PMs, Developers, and Developer Leads  should join Stackoverflow Forums that are located at [https://stackoverflow.microsoft.com](https://stackoverflow.microsoft.com)  to let us know if you have any questions. Remember to tag questions with ```ibiza``` or related tag.  For more information about the supported tags that are monitored by the Ibiza team, see [top-extensions-stackoverflow.md](top-extensions-stackoverflow.md).

* Developers who want to contribute to the Azure documentation or test framework should join groups from the site located at [http://aka.ms/azuregithub](http://aka.ms/azuregithub).

Ask an onboarding question on [Stackoverflow](https://stackoverflow.microsoft.com/questions/tagged/ibiza-onboarding).

## Get the SDK, docs, and samples to your developers

 The [development guide](top-extensions-getting-started.md) located in the main documentation index has all the right pointers.

# Phase 2 - Development

## Develop your extension

 The [development guide](top-extensions-getting-started.md) located in the main documentation index has all the right pointers.

## Learn about the hosting service / plan your deployment strategy

The Ibiza team provides and operates a common extension hosting service that makes it easy to get your extension into a globally distributed system without having to manage your own infrastructure. For more information see [top-extensions-hosting-service.md](top-extensions-hosting-service.md).

## Deployment using the Ibiza hosting service

For less common scenarios, you might need to do a custom deployment.

For example, if you need to talk to backend services using certificate-based authentication then you'll need controller code on the server. This is not supported with our hosting service. You should be very sure you require a custom hosting solution before going down this path. 

**NOTE**: The deployment can be configured in such a way that the client portion of the extension uses the hosting service while the custom controller code can be deployed separately.
For more information, see [portalfx-extensions-custom-deployment.md](portalfx-extensions-custom-deployment.md).

## Register the extension with the portal product configuration

Once the name of the extension is finalized, it is time to register the extension in all environments. This requires a portal deployment and can take time. Our Service Level Agreements are located at [portalfx-extensions-svc-lvl-agreements.md](portalfx-extensions-svc-lvl-agreements.md).  Please plan accordingly.

* For internal partners, the request to register an extension is a pull request, as specified in [portalfx-extensions-publishing.md](portalfx-extensions-publishing.md).
 
* External teams can submit their requests by reaching out to the <a href="mailto:ibizafxpm@microsoft.com?subject=Onboarding Request: Add <extensionName> to the Portal&body=Extension Name:  <br><br>Company:  <br><br>Brand or Suite:  <br><br>Product or Component:  <br><br> URLs: <br><br>Production: main.<extensionName>.ext.<company>.com<br><br>  Contact info: <br><br>Business Contacts <br><br> Dev leads: <br><br> PROD on-call email for live site incidents: <br><br>">ibizafxpm team</a> with an onboarding request.

* **NOTE**: Extension names must use standard extension name format, as in the example located at [portalfx-extensions-configuration-overview.md#name](portalfx-extensions-configuration-overview.md#name).

* **NOTE**:  Extension URLs adhere to the naming requirements located in [portalfx-extensions-cnames.md](portalfx-extensions-cnames.md).

* Enable the extension in all environments. 

# Phase 3 - Deployment

## Release kind

There are three typical release kinds. Private preview, public preview, and GA. For the purposes of deployment public preview and GA are the same. The only difference is that the UI may show preview labels and disclaimers where appropriate. For more information about the three kinds of releases, see  [top-extensions-developmentPhases.md](top-extensions-developmentPhases.md).

## Deploy the extension

1. Review the development phases that are located at [top-extensions-developmentPhases.md](top-extensions-developmentPhases.md) to understand how development is related to production-ready metrics criteria.

1. Review the environments that are specified in [portalfx-extensions-branches.md](portalfx-extensions-branches.md) to understand the environments in which the developer can test an extension.

1. Review the production-ready metrics that are specified in [top-extensions-production-ready-metrics.md](top-extensions-production-ready-metrics.md) to validate that the extension is ready for deployment.

1. If the extension requires additional built-in support for standard Graph or ARM APIs, submit a partner request at the site located at [https://aka.ms/portalfx/uservoice](https://aka.ms/portalfx/uservoice).  For information about other components that the new service needs, see [portalfx-extensions-contacts.md](portalfx-extensions-contacts.md).

1. When you are confident that the development of the extension is complete, execute the following process so that the specific work required for the Azure Fundamental tenets appears in Service360, as specified in [Azure Fundamentals](https://microsoft.sharepoint.com/teams/WAG/EngSys/Shared%20Documents/Argon/Azure%20Fundamentals%20Proposal/Azure%20Fundamentals%20Proposal.docx?d=wf5b821bc31c44042adb55ebf4d8b408d). 

    * Add the service to ServiceTree, which is located at [https://servicetree.msftcloudes.com](https://servicetree.msftcloudes.com)
    * Make the service be "Active" in ServiceTree
    * Complete metadata in ServiceTree to enable the automation for various Service360 Action Items
    * Complete the Action Items identified in Service360, which is located at [http://aka.ms/s360](http://aka.ms/s360)

1.  Request to deploy the extension to the Production environment, as specified in [portalfx-extensions-publishing](portalfx-extensions-publishing).

1. Integrate the extension into the Marketplace. 

    In the following images, each icon in the Azure Portal Marketplace is referred to as a Gallery item. Gallery items take the form of a file with the .azpkg extension. This is a  zip file which contains all assets for the gallery item: icons, screenshots, descriptions.

    ![alt-text](../media/portalfx-extensions-onboarding/azurePortalMarketPlace.png "Azure Portal Marketplace")

    * **PROD:** The Marketplace team accepts fully finished .azkpg files from your team and uploads them to Production to onboard the gallery package. Reach out to <a href="mailto:1store@microsoft.com?subject=Marketplace Onboarding Request&body=Hello, I would like to onboard the attached package to the production environment. The .azkpg package is named <packageName>. ">1store</a> with the zip file to have them install it.
    
    * **DOGFOOD:** Use AzureGallery.exe to upload items to DOGFOOD using the following command:

      ```AzureGallery.exe upload -p ..\path\to\package.azpkg -h [optional hide key]```

    In order to use the gallery loader, there are some values to set in the AzureGallery.exe.config file. For more information, see the Gallery Item Specifications document that is located at      [https://github.com/Azure/portaldocs/blob/master/gallery-sdk/generated/index-gallery.md#gallery-item-specificiations](https://github.com/Azure/portaldocs/blob/master/gallery-sdk/generated/index-gallery.md#gallery-item-specificiations).  

    For more dev/test scenarios, see [https://github.com/Azure/portaldocs/blob/master/gallery-sdk/generated/index-gallery.md#gallery-package-development-and-debugging-testing-in-production](https://github.com/Azure/portaldocs/blob/master/gallery-sdk/generated/index-gallery.md#gallery-package-development-and-debugging-testing-in-production).

You can ask developer community questions on Stackoverflow with the tag [ibiza-onboarding](https://stackoverflow.microsoft.com/questions/tagged/ibiza-onboarding).