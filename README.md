# Rag-demo
This project showcases the use of Retrieval-Augmented Generation (RAG) through OpenAI or Hugging Face APIs. You can run the notebooks in:

- **Google Colab**
- Or set up the project using Poetry in **VS Code**

## Google Colab Instructions

1. **Open Google Colab**

   https://colab.research.google.com/

   ![google_colab_open_notebook](/image/google_colab_open_notebook.png)

2. **Open notebook**

    Enter GitHub repository URL: [https://github.com/yuxuan-yx/rag-demo.git](https://github.com/yuxuan-yx/rag-demo.git). Select the notebook with the suffix `colab`.

   ![google_colab_select_notebook](/image/google_colab_select_notebook.png)

3. **Credentials**
    - If you are using the **OpenAI models**, input your credentials in the notebook:
        ```python
        OPENAI_BASE_URL = ""
        OPENAI_API_KEY = ""
        ```
    - For **Hugging Face models**, provide your Hugging Face token:
        ```python
        HF_TOKEN = ""
        ```
    - To obtain your Hugging Face token, follow the instructions here: https://huggingface.co/docs/hub/en/security-tokens

## VS Code instructions

Follow the instructions below to set up the project environment and dependencies.

### Prerequisites 

- **Miniconda**: An open-source package management and environment management system.

    - Download from: https://docs.anaconda.com/miniconda/install/#quick-command-line-install
- **Poetry**: A dependency management tool for Python.
    - Download instruction is in setup instructions - 3. **Install Poetry:**

- **VS Code**: Integrated development environment
    - Download from: 
    https://code.visualstudio.com/download

### Setup Instructions

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


### Adding Future Dependencies

To add new dependencies to the project, use the `poetry add` command followed by the package name. For example, to add the `requests` package, run:

```
poetry add requests
```
