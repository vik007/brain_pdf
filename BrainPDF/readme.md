# Introduction :
This is a Python application that allows you to load a PDF and ask questions about it using natural language. The application uses a LLM (Large Language Model) to generate a response about your PDF. The LLM will not answer questions unrelated to the document. if you ask any non related question then it will say "I dont know".

# How it works :
The application reads the PDF and splits the text into smaller chunks that can be then feed into a LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.
The application uses Streamlit to create the GUI and Langchain to deal with the LLM.

# pre-requisite :
  * Install python(version>2.7),and pip

# Installation :
To install the repository, please clone this repository and install the requirements:
 >> pip install -r requirements.txt

 You will also need to add your "OpenAI API key" to the .env file.

# Run Project :
To use the application, run the main.py file with the streamlit CLI (after having installed
streamlit):

>> streamlit run app.py
 