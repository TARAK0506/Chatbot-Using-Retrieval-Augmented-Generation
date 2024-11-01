##  RAG Application with Pinecone Serverless, Open Source LLMs and Embedding's, Langchain and Python.

### Project Overview

This chatbot assists users with information about their journeys, such as flight segments, seat details, layovers, and baggage allowances. It retrieves relevant details from a vector database, enriched by a generative model that interprets and answers complex travel-related questions.

### Key components:

Data Ingestion from JSON to a Pine Cone vector database for optimized retrieval.
Retrieval-Augmented Generation (RAG) for generating responses based on user queries.
Open Source LLMs and embeddings for language understanding and generation.

### Technologies used:

1. Groq Inference Engine

2. Vector Database - Pinecone Serverless

3. Embeddings - Hugging Face Transformers

4. Open Source LLMs - Llama3 & Mistral

5. Langchain Framework

6. Python
 


## Installation

1. **Clone the repository :**

   ```bash
    git clone https://github.com/TARAK0506/Chatbot-Using-Retrieval-Augmented-Generation.git
    cd RAG-Chatbot Using Langchain.
   ```
2. **Install dependencies** :
 Make sure Python is installed, then install the required packages:

   ```bash
    pip install -r requirements.txt
   ```
3. **Set up Environment Variables** :
   -  **Create an `.env` file** in the root directory.
   -  **Add necessary API keys** for Groq Inference Engine, Pinecone and Hugging Face in the following format:


      ```bash
      GROQ_API_KEY = your_pinecone_api_key
      PINECONE_API_KEY = your_pinecone_api_key
      HUGGINGFACE_API_KEY = your_huggingface_api_key
      ```

## Examples

### Sample Interaction

1. **Seat Details**
   - **User** : "What’s my seat for the first flight and the passenger details?"
   - **Bot** : 
     - **Passenger 1** : 
       - Full name: Surendra Singh 
       - Seat number: 21A
       - Cabin baggage allowance: 7kg
       - Check-in baggage allowance: 23kg

2. **Layover Information**
   - **User** : "Can you tell me about the layover time for my journey?"
   - **Bot** : "According to the ticket information, the layover duration for your flight is 55 minutes."

3. **Arrival Time**
   - **User** : "What time do I arrive in Delhi?"
   - **Bot** : "Your arrival at Indira Gandhi International Airport (DEL) in New Delhi is scheduled for 2024-07-12 at 08:10 AM."

4. **Baggage Allowance**
   - **User** : "Do I have checked baggage?"
   - **Bot** : "Yes, each passenger has a checked baggage allowance of 23kg for each flight segment."



## Limitations

   - Dependency on Data Quality: Accuracy relies on the quality of the ingested JSON data.
   - Limited Query Complexity: The RAG framework may struggle with highly complex or ambiguous queries without proper indexing.



## Future Improvements

   - **Expanding Query Capabilities :** Improve response accuracy for multi-part or ambiguous questions.
   
   - **Adding a Web Interface :** Consider a frontend UI for enhanced usability.
Enhanced Data Source Integration: Add more travel-related sources for richer responses.

   - **Enhanced Data Source Integration :** Add more travel-related sources for richer responses.



