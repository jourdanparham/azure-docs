---
title: "Quickstart: Image Analysis client library for Node.js"
description: Get started with the Image Analysis client library for Node.js with this quickstart
services: cognitive-services
author: PatrickFarley
manager: nitinme
ms.service: cognitive-services
ms.subservice: computer-vision
ms.topic: include
ms.date: 12/15/2020
ms.author: pafarley
ms.custom: devx-track-js
---

<a name="HOLTop"></a>

Use the Image Analysis client library for JavaScript to analyze a remote image for content tags.


> [!NOTE]
> You can also analyze a local image. See the [ComputerVisionClient](/javascript/api/@azure/cognitiveservices-computervision/computervisionclient) methods, such as **describeImageInStream**. Or, see the sample code on [GitHub](https://github.com/Azure-Samples/cognitive-services-quickstart-code/blob/master/javascript/ComputerVision/ImageAnalysisQuickstart.js) for scenarios involving local images.

> [!TIP]
> The Analyze API can do many different operations other than generate image tags. See the [Image Analysis how-to guide](../../Vision-API-How-to-Topics/HowToCallVisionAPI.md) for examples that showcase all of the available features.

[Reference documentation](/javascript/api/@azure/cognitiveservices-computervision/) | [Library source code](https://github.com/Azure/azure-sdk-for-js/tree/master/sdk/cognitiveservices/cognitiveservices-computervision) | [Package (npm)](https://www.npmjs.com/package/@azure/cognitiveservices-computervision) | [Samples](https://azure.microsoft.com/resources/samples/?service=cognitive-services&term=vision&sort=0)

## Prerequisites

* An Azure subscription - [Create one for free](https://azure.microsoft.com/free/cognitive-services/)
* The current version of [Node.js](https://nodejs.org/)
* Once you have your Azure subscription, <a href="https://portal.azure.com/#create/Microsoft.CognitiveServicesComputerVision"  title="Create a Computer Vision resource"  target="_blank">create a Computer Vision resource </a> in the Azure portal to get your key and endpoint. After it deploys, click **Go to resource**.
    * You will need the key and endpoint from the resource you create to connect your application to the Computer Vision service. You'll paste your key and endpoint into the code below later in the quickstart.
    * You can use the free pricing tier (`F0`) to try the service, and upgrade later to a paid tier for production.

## Setting up

### Create a new Node.js application

In a console window (such as cmd, PowerShell, or Bash), create a new directory for your app, and navigate to it.

```console
mkdir myapp && cd myapp
```

Run the `npm init` command to create a node application with a `package.json` file.

```console
npm init
```

### Install the client library

Install the `ms-rest-azure` and `@azure/cognitiveservices-computervision` NPM package:

```console
npm install @azure/cognitiveservices-computervision
```

Also install the async module:

```console
npm install async
```

Your app's `package.json` file will be updated with the dependencies.

Create a new file, *index.js*. 

### Find the subscription key and endpoint

[!INCLUDE [find key and endpoint](../find-key.md)]

## Analyze image

1. Open *index.js* in a text editor and paste in the following code.

   [!code-javascript[](~/cognitive-services-quickstart-code/javascript/ComputerVision/ImageAnalysisQuickstart-single.js?name=snippet_single)]


1. Paste your subscription key and endpoint into the code where indicated. Your Computer Vision endpoint has the form `https://<your_computer_vision_resource_name>.cognitiveservices.azure.com/`.

   > [!IMPORTANT]
   > Remember to remove the key from your code when you're done, and never post it publicly. For production, consider using a secure way of storing and accessing your credentials. See the Cognitive Services [security](../../../cognitive-services-security.md) article for more information.

1. Run the application with the `node` command on your quickstart file.

   ```console
   node index.js
   ```

## Clean up resources

If you want to clean up and remove a Cognitive Services subscription, you can delete the resource or resource group. Deleting the resource group also deletes any other resources associated with it.

* [Portal](../../../cognitive-services-apis-create-account.md#clean-up-resources)
* [Azure CLI](../../../cognitive-services-apis-create-account-cli.md#clean-up-resources)

## Next steps

In this quickstart, you learned how to install the Image Analysis client library and make basic image analysis calls. Next, learn more about the Analyze API features.

> [!div class="nextstepaction"]
>[Call the Analyze API](../../Vision-API-How-to-Topics/HowToCallVisionAPI.md)

* [Image Analysis overview](../../overview-image-analysis.md)
* The source code for this sample can be found on [GitHub](https://github.com/Azure-Samples/cognitive-services-quickstart-code/blob/master/javascript/ComputerVision/ImageAnalysisQuickstart.js).

