# Foundry _Getting Started_: Using a Model

This is a Python/Jupyter-based project for getting started using Microsoft Foundry with AI models.

Two dependencies are required: `azure-ai-projects` and `azure-identity`. All others are Jupyter-related.

## ENTRA-ID BRANCH - ALTERNATIVE IMPLEMENTATION

As the previous [branch](#), this uses Entra ID instead of API key. However, this implementation introduces changes, as follows:
- Importing `AIProjectClient` class;
- Creating project configuration with `endpoint` and `credentials`; and,
- Getting the client through `get_openai_client`

This implementation avoids hard-coding the suffix. But, the main benefit is that `AIProjectClient` is the Foundry project control plane — listing deployments, resolving connections, managing agents and indexes, wiring up evaluations. The raw OpenAI client reaches none of it; it only speaks the inference API.