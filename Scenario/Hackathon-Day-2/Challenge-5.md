# Challenge 05: Serverless Document Batch Processing 

### Estimated Time: 90 minutes

## Introduction:

Welcome to a pivotal challenge where Contoso Ltd. aims to enhance its AI-powered chat app with a robust document processing system. This challenge focuses on creating a serverless solution for processing new documents, translating them as needed, and seamlessly storing them into Azure AI Search. This system will ensure that these documents are continuously available for consumption by Azure OpenAI, enhancing the chat app's knowledge base and response accuracy.

Building on your previous achievements in load-balancing Azure OpenAI resources, you will now embark on a journey to streamline document processing. This involves setting up a translation service, creating a serverless architecture for batch processing using Azure services, and leveraging technologies like Form Recognizer and Azure AI Search. Your task is to ensure that newly added documents are promptly processed, analyzed, and indexed, making them readily available for the chat app's AI to utilize.

This challenge unfolds in three main stages: language translation, serverless document batch processing using Azure services, and leveraging advanced features like Form Recognizer and AI search. We kick things off by translating files to meet language requirements. Next, you deploy a serverless architecture, utilizing Azure services, for efficient batch processing of documents. You train and test our model, establish a pipeline to convert documents into a Form Recognizer format, and bring in Azure's AI search service to verify the presence of specific documents in the processed dataset from where they can be used by Azure OpenAI. 

You will utilize the Form Recognizer Service and the Business Process Automation (BPA) Accelerator to build pipelines across various Azure services, creating a seamless document processing solution. This challenge is a step towards realizing an AI solution that can adapt and grow with Contoso's business needs.

## Challenge Objectives:

> **Important**: When deploying services in this challenge, please make sure to use the resource group named **<inject key="Resource Group Name"/>**  !

1. **Fork the repository and generate a GitHub Personal Access Token (PAT).**

   - Fork the **Business Process Automation** repository into your GitHub: `https://github.com/Azure/business-process-automation`.
   - Generate a GitHub **Personal Access Token (PAT)** with Workflow Level Token.

1. **Deploy Azure Infrastructure in the Azure Portal**:

   - Click on the "Deploy to Azure" button (TODO):

      [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fbusiness-process-automation%2Fmain%2Ftemplates%2Foneclickoai.json)

   - Update the repository token and forked Git repository URL while leaving all other settings unchanged.

1. **Install dependencies and translate typescript**.

      - Clone the repository and change the directory to `src/backend/api`.
      - Execute **npm** to build the project.

1. **Deploy functions in the Azure Function App**.
      
      - Ensure to stay in the api directory and publish the function.

    > **Hint**: Publish the function to the designated function app that is configured to use the JavaScript runtime stack.
    
    > **Note**: Make sure you are logged in to Azure
        
   - Change the directory to `\src\backend\huggingface` and publish the function.

    > **Hint**: Publish the function to the designated function app that is configured to use the Python runtime stack.

1. **Setup Azure Blob Storage.**
   - Create mandatory source and target containers in Azure Blob Storage for document processing by granting blob access.

1. **Initialize the C#/.NET Environment for Document Processing:**
   - Set up a C#/.NET project in Visual Studio for document translation using .Net Version 7.
   - Install the necessary packages, including Newtonsoft.Json.


1. **Translate Documents and Run the Application:**
   - Implement document translation code in the C#/.NET project.
   - Execute the application to translate all documents in the storage container.
   > Note: You can find the documents in C:\LabFiles\Documents.


   <validation step="6936c21b-ffd6-4778-904b-25346932940b" />

**Using Doc Intelligence:**
> **Important**: When deploying services in this challenge, please make sure to use the resource group named **<inject key="Resource Group Name"/>**  !

1. **Using an Azure Document Intelligence (Form Recognizer) resource:**
    - Navigate to Azure AI services and utilize the Azure Document Intelligence (Form Recognizer) resource.
    - Upload and label training documents to train the Azure Document Intelligence (Form Recognizer) model.
    > Note: You can find the documents in C:\LabFiles\Documents.


2. **Build a New Pipeline with a Custom Model Module in BPA:**
    - Utilize the trained Azure Document Intelligence  to create a new pipeline in BPA.
    - Configure the pipeline for efficient document processing and integration with Azure Cognitive Search.
    > Hint : Utilize static web app.


3. **Configure Azure AI Search:**
    - Connect to Azure Blob Storage and configure data import and indexing.
    - Set up an indexer for organized data retrieval.


4. **Update the Azure OpenAI Model to use the Azure AI Search**
    - Update your existing Azure OpenAI model deployment to connect to the newly created AI Search index and test using the Azure OpenAI Playground.
      
## Success Criteria:

- Successful translation of documents and storage in the Azure Blob Storage target container.
- Effective setup and utilization of the Form Recognizer resource and BPA pipeline.
- Proper configuration of Azure Cognitive Search for processed documents.
- Validation of document processing and search functionality using the Sample Search Application in BPA.

## Additional Resources:

- Refer to [document translation](https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/quickstarts/document-translation-rest-api?pivots=programming-language-csharp#code-sample) for sample code that will be used for document translation using C#.
- Refer to [Document Translation operations](https://learn.microsoft.com/en-us/azure/ai-services/translator/document-translation/reference/rest-api-guide) to understand the REST APIs that we utilize for document translation.
