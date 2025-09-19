# Conversation Management & Classification using Groq API

This repository contains a Google Colab notebook that demonstrates two primary tasks using the Groq API (OpenAI-compatible interface):

1. **Conversation Management (Truncation & Summarization)**  
   - Manage long chat histories by truncating them by turns, characters, or words.  
   - Implement periodic summarization every *k* runs, replacing history with a summary.  

2. **Conversation Classification with JSON Schema & Function Calling**  
   - Use structured extraction (OpenAI-compatible function-calling) to classify chats and extract user details into a strict JSON Schema.  
   - Validate results using `jsonschema`.  

---

## Features

- No frameworks (Streamlit, Flask, etc.) — only standard Python + `requests` or OpenAI-compatible SDK.  
- Demonstrations are copy-paste runnable in Colab.  
- API key is requested securely via `.env` or `getpass`.  
- Includes unit-style tests and clear printed outputs at each stage.  

---

## Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/Convo_management.git
   cd Convo_management
2. Install the required packages:
   ```bash 
   pip install -r requirements.txt

3. Configure your environment variables:

 -  Copy .env.example to .env
 -  Add your Groq API key inside .env
Example:
    ```bash
       GROQ_API_KEY=your_api_key_here

## Usage
Running in Google Colab

- Open the notebook (notebook.ipynb) in Colab.

- When prompted, enter your Groq API key securely.

- Run cells sequentially to test both tasks (conversation management and classification).

Running Locally

- Make sure you have Python 3.9+ installed.

- Launch Jupyter Notebook or Jupyter Lab:
  ```bash
  jupyter notebook

- Open notebook.ipynb and run cells.
## Files

- `notebook.ipynb` :	Main Google Colab notebook with full implementation.
- `.env.example` :	Example environment file (rename to .env and add your Groq API key).
- `requirements.txt` : 	Python dependencies required to run the notebook.
- `.gitignore` :	Ensures sensitive files like .env are not committed.
- `README.md` :	Project documentation.
- `LICENSE` : 	License file (MIT by default).

## Dependencies

`openai` (Groq-compatible client)

`requests` (API calls fallback)

`jsonschema` (schema validation)

See `requirements.txt` for the full list.

