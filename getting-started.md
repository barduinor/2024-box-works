# Getting Started
Follow these steps to get started with the workshop.

## Prerequisites

To successfully complete this workshop, ensure you have the following:

- A Box account with access to the Box AI API.
- A Box CCG application created in your Box account (see this [guide](https://medium.com/box-developer-blog/box-python-next-gen-sdk-getting-started-with-ccg-81be0abc82d9)).
- Python 3.9 or higher installed on your machine.

Follow our official guide to [Get started with Box AI](https://developer.box.com/guides/box-ai/prerequisites/).

## Clone the Repository:

```bash
git clone git@github.com:box-community/Box-AI-Workshop.git
cd Box-AI-Workshop
```

## Create a python virtual environment:

### On MacOS and Linux (Python 3.12)
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
### On Windows CMD (Python 3.12)
```bash
python3 -m venv .venv
.venv\Scripts\activate.bat
pip install --upgrade pip
pip install -r requirements.txt
```

### On Windows PowerShell (Python 3.12)
```bash
python3 -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

## Set Up Your Environment:

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

## Initialize the Box AI Workshop:

Run the `gen_sample_data.py` script to generate sample data in your Box account:

```bash
python src/gen_sample_data.py
```

You should see a summary of your configurations and the sample data being generated in your Box account.


