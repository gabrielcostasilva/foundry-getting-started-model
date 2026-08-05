# Foundry _Getting Started_: Using a Model

This is a Python/Jupyter-based project for getting started using Microsoft Foundry with AI models.

Two dependencies are required: `azure-ai-projects` and `azure-identity`. All others are Jupyter-related.

## OPENAI-CLIENT BRANCH

As the previous [branch](https://github.com/gabrielcostasilva/foundry-getting-started-model/tree/entra-id), this uses Entra ID instead of API key. However, this implementation uses the OpenAI client, which introduces the following changes:
- Importing `AIProjectClient` class;
- Creating project configuration with `endpoint` and `credentials`; and,
- Getting the client through `get_openai_client`

This implementation avoids hard-coding the suffix. But, the main benefit is that `AIProjectClient` is the Foundry project control plane — listing deployments, resolving connections, managing agents and indexes, wiring up evaluations. The raw OpenAI client reaches none of it; it only speaks the inference API.