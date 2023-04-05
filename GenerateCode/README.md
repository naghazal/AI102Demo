# Generative AI Demo using Azure Cognitive Services and OpenAI GPT-3

This demo showcases how to generate code snippets for a given programming task using **Azure Cognitive Services** and **OpenAI GPT-3**. The solution uses the Azure Cognitive Services Text Analytics API to extract the requirements and constraints from a given task description, and then uses the OpenAI GPT-3 API to generate code snippets that fulfill those requirements and constraints.

## Step-by-Step Guide

Follow these steps to implement the generative AI solution using Azure and OpenAI APIs:

### Step 1: Set up Azure Cognitive Services

1. Sign in to the **Azure portal** with your account.
2. Click on the "Create a resource" button and search for "CognitiveServices".
3. Click on the "Create" button.
4. Fill in the required details, such as the resource group, name, location, pricing tier, etc.
5. Once the CognitiveServices is created, note down the API key and endpoint URL.

### Step 2: Set up Azure OpenAI GPT-3 API

1. Choose the OpenAI API: For this demo, we'll be using the GPT-3 API, which is a state-of-the-art language generation model. Deploy the "code-davinci-003" model.
2. Authenticate the API: You'll need to provide your subscription key, which you can find in the Azure portal.

### Step 3: Set up a development environment

1. Write the code: You can find the code [here](GenerateCode.ipynb).
2. Test the chatbot: Use tools like Postman or cURL to send HTTP requests to the API and see the responses.

Note that you need to replace `<your-subscription-key>`, `<your-endpoint-url>`, `<your-openai-api-key>`, and `<your-openai-endpoint-url>` with your actual API key and endpoint URL values. Also, the above code generates only one code snippet, but you can modify the `n` parameter in the OpenAI API request to generate multiple code snippets.
