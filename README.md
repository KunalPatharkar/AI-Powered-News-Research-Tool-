# AI-Powered News Research Tool 📰🤖  

An AI-powered news research tool built for effortless information retrieval and financial insights. It enables users to load article URLs or upload text files containing multiple URLs, processes the content into embeddings, and allows interactive Q&A through ChatGPT with source references.  


## ✨ Features  

- **Fetch News Content**: Load URLs or upload text files containing article links to gather news automatically.  
- **Smart Processing**: Process article text using **LangChain’s UnstructuredURL Loader**.  
- **AI Embeddings**: Convert content into embeddings with **OpenAI’s embeddings**.  
- **Fast Search**: Store vectors in a **FAISS database** for efficient similarity search and retrieval.  
- **Ask & Answer**: Interact with **ChatGPT** by asking questions and receive accurate responses along with source URLs.  

## 🚀 Installation   

1.Clone this repository to your local machine using:

```bash
  git clone https://github.com/KunalPatharkar/AI-Powered-News-Research-Tool.git
```
2.Navigate to the project directory:

```bash
  cd AI-Powered-News-Research-Tool
```
3. Install the required dependencies using pip:

```bash
  pip install -r requirements.txt
```
4.Set up your OpenAI API key by creating a .env file in the project root and adding your API

```bash
  OPENAI_API_KEY=your_api_key_here
```
## Usage/Examples

1. Run the Streamlit app by executing:
```bash
streamlit run main.py

```

2.The web app will open in your browser.

- On the sidebar, you can input URLs directly.

- Initiate the data loading and processing by clicking "Process URLs."

- Observe the system as it performs text splitting, generates embedding vectors, and efficiently indexes them using FAISS.

- The embeddings will be stored and indexed using FAISS, enhancing retrieval speed.

- The FAISS index will be saved in a local file path in pickle format for future use.
- One can now ask a question and get the answer based on those news articles

  - https://www.moneycontrol.com/news/business/tata-motors-mahindra-gain-certificates-for-production-linked-payouts-11281691.html
  - https://www.moneycontrol.com/news/business/tata-motors-launches-punch-icng-price-starts-at-rs-7-1-lakh-11098751.html
  - https://www.moneycontrol.com/news/business/stocks/buy-tata-motors-target-of-rs-743-kr-choksey-11080811.html

## Project Structure

- main.py – Streamlit app entry point
- requirements.txt – List of required Python packages
- faiss_store_openai.pkl – Local FAISS index storage
- .env – Configuration file containing your OpenAI API key