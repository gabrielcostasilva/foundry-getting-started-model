# Foundry _Getting Started_: Using a Model

This is a Python/Jupyter-based project for getting started using Microsoft Foundry with AI models.

Two dependencies are required: `azure-ai-projects` and `azure-identity`. All others are Jupyter-related.

## ENTRA-ID BRANCH

This branch uses Entra ID instead of API key - usefull for fine-grained permissions.

However, there are prerequisites to use it. First, [install the Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest). Second, update the `token_provider`. Then, update the `base_url` appending `/openai/v1`. Finally, runs `az login` to login to your Azure account. 



