# Box AI Workshop

Welcome to the Box AI Workshop! This repository contains a comprehensive guide for developers to utilize the Box AI endpoints through the Box Python Next Gen SDK. In this workshop, you'll learn how to interact with various Box AI capabilities, including document processing and conversational interactions with a language model.

## Workshop Overview

In this workshop, we will cover the following Box AI endpoints:

1. **`/ai/ask`**: Engage with single and multiple documents to retrieve information.
2. **`/ai/textgen`**: Facilitate conversational interactions with a language model (LLM) across one or multiple documents.
3. **`/ai/extract`**: Extract data from documents in an intuitive manner.
4. **`/ai/extract_structured`**: Utilize a formal description for output structure to enhance data extraction accuracy.

## Prerequisites

To successfully complete this workshop, ensure you have the following:

- A Box account with access to the Box AI API.
- Python 3.9 or higher installed on your machine.

## Getting Started
Follow these steps to get started with the workshop:

### Clone the Repository:

bash
Copy code
git clone https://github.com/box-community/box-ai-workshop.git
cd box-ai-workshop

### Create a python virtual environment:

#### On MacOS and Linux (Python 3.12)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
#### On Windows CMD (Python 3.12)
```bash
python3 -m venv .venv
.venv\Scripts\activate.bat
pip install --upgrade pip
pip install -r requirements.txt
```

#### On Windows PowerShell (Python 3.12)
```bash
python3 -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

### Set Up Your Environment:

Create a .env file in the root directory of the project and add your Box API credentials:

```
# CCG settings
BOX_CLIENT_ID = YOUR_CLIENT_ID
BOX_CLIENT_SECRET = YOUR_CLIENT_SECRET

BOX_ENTERPRISE_ID = YOUR_ENTERPRISE_ID
BOX_USER_ID = YOUR_USER_ID

FOLDER_SAMPLES = demo/samples
BOX_ROOT_DEMO_FOLDER = YOUR_ROOT_FOLDER_ID_TO_STORE_SAMPLES
```

### Initialize the Box AI Workshop:

Run the `gen_sample_data.py` script to generate sample data in your Box account:

```bash
python src/gen_sample_data.py
```

You should see a summary of your configurations and the sample data being generated in your Box account.


