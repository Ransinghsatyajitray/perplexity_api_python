# perplexity_api_python
This repository is on testing the perplexity api and how it can aid in giving upto date answer to the query

# Step to follow
1. Create an account in perplexity ai. Visit the Perplexity website and create an account if you don’t already have one.
2. Navigate to the API settings page at Perplexity API Settings.
3. Enter your billing information to set up a payment method. This step is necessary to generate an API key.
4. In the API settings, locate the “Available Credits” section and click “Buy Credits.”
5. Enter the amount of credits you want and follow the prompts to complete the transaction.
6. Once billing information is set and credits are purchased, go to the “API Keys” section in your account dashboard (should be below the Credits).
7. Click the “Generate API Key” button to create your API key. This key will be a long string of characters.
8. Treat your API key like a password. Do not share it publicly or expose it in your code repositories.
9. Set the keys in the .env file and export that to the notebook using the load_dotenv from dotenv
10. Got to https://docs.perplexity.ai/api-reference/chat-completions  (there is a copy option beside send). This is the url which we need to pass to the request body to the preplexity ai api
11. Other than the above we require the header which essentially include the API key, the body which include the model and its parameter and the system & user role and their respective message
12. The output is a requests.models.Response object whose choices field contains the necessary answer. 
13. if we want to convert the response to json format we can use response.json
    
