# Foundry _Getting Started_: Using a Model

This is a Python/Jupyter-based project for getting started using Microsoft Foundry with AI models.

Two dependencies are required: `azure-ai-projects` and `azure-identity`. All others are Jupyter-related.

## INPUT ARRAY BRANCH

This branch replaces the traditional `string` input with a structured array. Notice that this **is not** a simple syntax sugar. The string format optimizes for fast prototyping and clean single-turn/text-only execution, while the array format is useful for multimodal inputs and multi-step AI agents.

> Also notice we are using `load_dotenv()` to load env variables.