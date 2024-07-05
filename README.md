

# Medical Chat Bot 🩺

Medical Bot is a powerful tool designed to provide medical information by answering user queries using state-of-the-art language models and vector stores.

## Table of Contents

- [Introduction](#langchain-medical-bot)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Usage](#usage)

## Prerequisites

Before you can start using the Medical Bot, make sure you have the following prerequisites installed on your system:

- Python 3.6 or higher
- Required Python packages (you can install them using pip):
    - langchain
    - chainlit
    - sentence-transformers
    - faiss
    - PyPDF2 (for PDF document loading)

## Installation

1. Clone this repository to your local machine.

    ```bash
    git clone https://github.com/Rajan-Okita/Medical_chatbot.git
    ```

2. Create a Python virtual environment (recommended):

    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```

3. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Set up the necessary paths and configurations in your project, including the `DB_FAISS_PATH` variable and other configurations as per your needs.

## Getting Started

To get started with the Medical Bot, you need to:

1. Set up your environment and install the required packages as described in the Installation section.

2. Configure your project by updating the `DB_FAISS_PATH` variable and any other custom configurations in the code.
3. Run ingest file to set up the vectorstore folder:
   ```bash
    python ingest.py 
    ```
4. Prepare the language model and data as per the Langchain documentation.

5. Start the bot by running the provided Python script or integrating it into your application.
   ```bash
    chainlit run main.py -w 
    ```
    
## Usage

The Medical Bot can be used for answering medical-related queries. To use the bot, you can follow these steps:

1. Start the bot by running your application or using the provided Python script.

2. Send a medical-related query to the bot.

3. The bot will provide a response based on the information available in its database.

4. If sources are found, they will be provided alongside the answer.

5. The bot can be customized to return specific information based on the query and context provided.