# Using Azure Credits

This repo contains scripts to get started with using the Azure credits we have for KLab. They expire at the end of June, and we have ~$20,000 worth.

## Azure Setup

The Azure_setup.ipynb file has scripts to get you started. First you will need to make environment variables for `AZURE_OPENAI_API_KEY` and `AZURE_OPENAI_ENDPOINT`. 

I recommend using the dotenv library (install as `pip install python-dotenv`). Then make a file called .env in your workspace. But then you will also need to create a .gitignore file to avoid pushing it to the repo if you want to make updates.

### LLM API Calls

We only have access to OpenAI models. And among the GPT-4 models, we seem to only have access to GPT-4o. I could create a deployment to use GPT-3.5 or GPT-3.5-turbo, but I'm assuming no one wants to use these, so I will hold off on even making that an option.

Because GPT-4o is designed for chat, prompts submitted to the API must follow the "role" / "content" format given in the example. If you want, you can prompt the model with a conversation that is already multiple turns deep (as in the example).

### Embedding API Calls

You can also use the Azure credits to get embedding vectors from OpenAI. They do sentence-level (or even paragraph level?) embeddings.




