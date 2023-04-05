# AI Chatbot using Azure OpenAI APIs

## Demo Idea:

The demo idea is to create an AI-powered chatbot that can communicate with users in natural language. The chatbot will be able to generate responses that are tailored to the user's input using Azure OpenAI APIs.

## Tools:

- Azure Openai service
- Python
- Colab

## Step-by-Step Guide:

1. Set up an Azure account: First, you'll need to set up an Azure account if you don't already have one. You can sign up for a free account or a paid subscription depending on your needs.

2. Create a Cognitive Services resource: Next, you'll need to create a Cognitive Services resource in Azure. This resource will provide access to the Azure OpenAI APIs that you'll be using for the chatbot.

3. Choose the OpenAI API: There are several Azure OpenAI APIs to choose from, but for this demo, we'll be using the GPT-3 API, which is a state-of-the-art language generation model. Deploy "code-davinci-003" model.

4. Authenticate the API: Once you've chosen the API, you'll need to authenticate it so that you can make requests to it from your code. You'll need to provide your subscription key, which you can find in the Azure portal.

5. Set up a development environment: You'll need to set up a development environment to write the code for the chatbot. You can use any programming language that supports HTTP requests, such as Python or Node.js. You can use Colab (https://colab.research.google.com/) to run the code.

6. Write the code: You can find the code [here](code.py).

7. Test the chatbot: You can test the chatbot to make sure it's working correctly. You can use tools like Postman or cURL to send HTTP requests to the API and see the responses.

With these steps, you can implement a generative AI solution that uses Azure OpenAI APIs to generate natural language responses for a chatbot.

## Details:

In this code, we first set up the OpenAI API credentials and configuration at the beginning of the code. Then, we define the `get_response` function using the `openai` library, which we call whenever we need to get a response from the OpenAI API.

Finally, we define the `chat` function, which handles the conversation with the user. Whenever the user enters input, we call the `get_response` function to get a response from the OpenAI API, and then print the response to the console.

To use this code in your Colab notebook, you'll need to replace "YOUR_OPENAI_API_KEY" with your own API key for the OpenAI API. You can find your API key in your OpenAI dashboard.

## Notes:

- If you're getting a `ModuleNotFoundError` for the `openai` module, it means that the module is not installed on your system. To use the OpenAI API in your Python code, you'll need to install the `openai` Python module.

You can install the `openai` module using pip, which is a package manager for Python. Here's how you can install the `openai` module:

pip install openai

Wait for the installation to complete. Once the installation is complete, you should be able to import the openai module in your Python code.
After installing the openai module, try running your code again and see if the error goes away.


- If you're getting an InvalidRequestError with the message "The API deployment for this resource does not exist", it means that the API deployment may not have been successfully created or is not yet fully provisioned.

- If you created the API deployment within the last 5 minutes, the error message suggests waiting a few minutes and trying again.

- If you still encounter the error message after waiting a few minutes, you can try the following steps:

1. Double-check that you have correctly followed the steps for deploying your API to Azure and that you have provided all the required information, including the API key, endpoint, and resource group.

2. Check that the resource group you specified when deploying the API exists and that the resource is deployed within that resource group.

3. Verify that the API endpoint URL you are using is correct and that there are no typos or errors in the URL.

4. Check that the API deployment is not in a failed state by checking the Azure portal or using the Azure CLI.

If none of these steps work, you can try deleting the API deployment and recreating it from scratch.
