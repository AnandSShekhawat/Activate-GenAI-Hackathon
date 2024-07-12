# Challenge 1: Deploy Azure OpenAI Service and LLM Models

### Estimated Time: 30 minutes

## Introduction

**Azure OpenAI Service** provides REST API access to OpenAI's powerful language models, including the GPT-4, GPT-4 Turbo with Vision, `gpt-35-turbo`, and Embeddings model series. In addition, the new `GPT-4` and `gpt-35-turbo` model series have now reached general availability.

A **Large Language Model (LLM)** is a deep learning algorithm that can perform a variety of natural language processing (NLP) tasks. Large language models use transformer models and are trained using massive datasets—hence, large. This enables them to recognize, translate, predict, or generate text or other content.

**Contoso Ltd.**, a leading technological firm, is seeking to enhance its product support operations. They receive a vast number of queries daily, which results in longer waiting times and decreased customer satisfaction. To address this, Contoso is planning to implement an AI-powered solution that can handle customer inquiries effectively and efficiently.

They have chosen to deploy Azure OpenAI Service along with its Large Language Models (LLM), like `gpt-35-turbo` and `text-embedding-ada-002`. These models are known for their capability in processing and generating human-like text, making them ideal for this application.

As a part of this challenge, your task is to create an Azure OpenAI service and deploy Large Language Models (LLM). The LLMs include **gpt-35-turbo** and **text-embedding-ada-002**.

### Accessing the Azure portal

1. To access the Azure portal, open a private/incognito window in your browser and navigate to the Azure Portal.

1. On the **Sign in to Microsoft Azure tab**, you will see a login screen. Enter the following email/username, and then click on **Next**.

   - **Email/Username:** <inject key="AzureAdUserEmail"></inject>

1. Now enter the following password and click on **Sign in**.

   - **Password:** <inject key="AzureAdUserPassword"></inject>

1. If you see the pop-up **Stay Signed in?**, click No.

1. If you see the pop-up **You have free Azure Advisor recommendations!**, close the window to continue with the challenge.

1. If a **Welcome to Microsoft Azure** pop-up window appears, click **Maybe Later** to skip the tour.

## Prerequisites

Make sure you have the following from the CloudLabs-provided integrated environment:

> Note: Prerequisites are already set up in the CloudLabs-provided environment. If you're using your personal computer or laptop, please make sure that all necessary prerequisites are installed to complete this hackathon.

  - [Azure Subscription](https://azure.microsoft.com/en-us/free/)
  - [Azure OpenAI](https://aka.ms/oai/access) access is available with the following models:
    - gpt-35-turbo
    - text-embedding-ada-002

## Challenge Objectives:

1. **Azure OpenAI Service Deployment:**
   - Set up an Azure OpenAI Service instance with SKU size Standard `S0`.
   - Deploy it in the existing resource group named - **<inject key="Resource Group Name"/>**
   - Obtain the necessary Azure OpenAI Key and Endpoint.

   <validation step="ccff4a0f-eb81-479e-a774-00cc5a664eeb" />

2. **Deploy Large Language Models (LLM):**
   - Azure OpenAI provides a web-based portal named **Azure OpenAI Studio** that you can use to deploy, manage, and explore models. You'll start your exploration of Azure OpenAI by using Azure OpenAI Studio to deploy a model.
   - Launch Azure OpenAI Studio from the overview pane and deploy two OpenAI models, i.e., `gpt-35-turbo` and `text-embedding-ada-002`, with a TPM capacity of 20k.

   <validation step="32bbf48f-1030-4e8b-8dfe-a395a6746f1d" />

## Success Criteria:

- Verify that the Azure OpenAI Service is successfully deployed in the existing resource group - <inject key="Resource Group Name"/>.
- Verify that the Large Language Models (LLM), `gpt-35-turbo` and `text-embedding-ada-002`, are successfully deployed with the Azure OpenAI Service.

## Additional Resources:

- Refer to the [Azure OpenAI Service documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/) for guidance on deploying the service.

### Challenge Validation
 
1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 

     ![azure](../media/validate01.png)
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!** This means that you have successfully completed the challenge.
 
   ![azure](../media/validate02.png)
   
1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
   ![azure](../media/validate03.png)
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
   
   ![azure](../media/validate04.png)
   
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

### Conclusion

In this challenge, you’ve effectively validated the Azure OpenAI service and deployed LLM models. In the next challenge, you will learn about Document Search.
