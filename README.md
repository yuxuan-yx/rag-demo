# Project Setup

This project demonstrates the use of Retrieval-Augmented Generation (RAG) models using either OpenAI or Hugging Face APIs. Follow the instructions below to set up the project environment and dependencies.

## Prerequisites

- **Conda**: An open-source package management and environment management system.
- **Poetry**: A dependency management tool for Python.
- **VSCode** (optional): Recommended for working with Jupyter Notebooks.

## Setup Instructions

1. **Create a Conda environment:**

    First, create a new Conda environment named `rag-demo-env` with Python 3.11:

    ```sh
    conda create -n rag-demo-env python=3.11
    ```

2. **Activate the Conda environment:**

    Activate the newly created Conda environment:

    ```sh
    conda activate rag-demo-env
    ```

3. **Install Poetry:**

    Poetry is used for dependency management.

    ```sh
    pip install poetry
    ```

4. **Install project dependencies:**

    Navigate to the root directory of the project and install the dependencies using Poetry:

    ```sh
    poetry install
    ```

5. **Create .env file:**

    Create a  file in the root directory by following the structure provided in `.env.example`. Depending on the API you are using, add the necessary keys:

    - For OpenAI API:
      ```
      OPENAI_BASE_URL = ""
      OPENAI_API_KEY = ""
      ```

    - For Hugging Face models:
      How to get your Hugging Face token: https://huggingface.co/docs/hub/en/security-tokens
      ```
      HF_TOKEN = ""
      ```

5. **Install project dependencies:**

    Navigate to the root directory of the project and install the dependencies using Poetry:

    ```sh
    poetry install
    ```

## Adding Future Dependencies

To add new dependencies to the project, use the `poetry add` command followed by the package name. For example, to add the `requests` package, run:

```
poetry add requests
```