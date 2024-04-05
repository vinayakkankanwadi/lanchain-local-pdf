# Langchain Ask PDF (Tutorial)

This is a Python application that allows you to load a PDF and ask questions about it using natural language. The application uses a LLM to generate a response about your PDF. The LLM will not answer questions unrelated to the document.

## How it works

The application reads the PDF and splits the text into smaller chunks that can be then fed into a stable-vicuna through LlamaCpp LLM model. It uses all-MiniLM-L6-v2 embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.

The application uses Streamlit to create the GUI and Langchain to deal with the LLM.


## Installation

To install the repository, please clone this repository and install the requirements:

```
pip install -r requirements.txt
```

## Usage

To use the application, run the `app.py` file with the streamlit CLI (after having installed streamlit): 

```
streamlit run app.py
```

## Demo

When the app is run, one should can upload any pdf and ask question on the same.

![image](https://raw.githubusercontent.com/vinayakkankanwadi/lanchain-local-pdf/main/screenshot.JPG)

## Contributing

This repository is for educational purposes only and is not intended to receive further contributions. 
