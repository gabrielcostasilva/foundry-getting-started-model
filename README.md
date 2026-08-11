# Foundry _Getting Started_: Using a Model

This is a Python/Jupyter-based project for getting started using Microsoft Foundry with AI models.

Two dependencies are required: `azure-ai-projects` and `azure-identity`. All others are Jupyter-related.

> Notice that in [this commit](https://github.com/gabrielcostasilva/foundry-getting-started-model/commit/d0e37ace8ccc8e477ca31e84b7db260af3c6d87c) we replaced hard-coded strings with env variables. This is the standard for keys and addresses. 

## Branches

Other branches extend this project as follows:
- [entra-id](https://github.com/gabrielcostasilva/foundry-getting-started-model/tree/entra-id) replaces the API token with Entra ID credentials;
- [openai-client](https://github.com/gabrielcostasilva/foundry-getting-started-model/tree/openai-client) uses the OpenAI client, which give access to other features.
- [setting-parameters](https://github.com/gabrielcostasilva/foundry-getting-started-model/tree/setting-parameters) adds inference parameters to customise the response.
