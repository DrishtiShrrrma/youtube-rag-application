**Start: YouTube RAG Application Process**

|
|--> **scrapetube Initialization**
|    |
|    |--> Input YouTube Channel URL (e.g., youtube.com/@nameofchannel)
|    |--> **Output**: Initial connection to YouTube
|
|--> **Data Retrieval Process**
|    |
|    |--> **scrapetube**: Retrieves list of videos from YouTube channel
|    |    |
|    |    |--> Send HTTP GET Request to YouTube to fetch video metadata
|    |    |--> **Output**: Video metadata and list of videos
|
|--> **YouTube Interaction**
|    |
|    |--> **scrapetube** communicates with **YouTube**
|    |--> YouTube provides metadata through HTTP GET requests
|    |
|    |--> **Output**: Acquired metadata for each video on the list
|
|--> **youtube-transcript-api Processing**
|    |
|    |--> Process each video metadata through **youtube-transcript-api**
|    |    |
|    |    |--> Fetch video transcripts (if available)
|    |    |--> Generate a TXT file for each transcript
|    |
|    |--> **Output**: Transcript saved in TXT format for each video
|
|--> **Text Extraction and Preprocessing**
|    |
|    |--> Extract text data from various file types (PDF, PPT, TXT)
|    |--> Split text data into chunks for processing
|
|--> **Embedding Generation**
|    |
|    |--> Create embeddings for each text chunk
|    |--> Store embeddings in **Qdrant Vector DB**
|
|--> **Retrieval Process**
|    |
|    |--> Query Qdrant Vector DB for top-k relevant chunks
|    |    |
|    |    |--> Retrieve relevant chunks based on embeddings
|    |
|    |--> **Output**: Top-k relevant chunks for the query
|
|--> **LLM Processing**
|    |
|    |--> Feed retrieved chunks to **LLM (Large Language Model)**
|    |--> Generate a response based on retrieved context
|
|--> **Final Output Generation**
|    |
|    |--> Consolidate and format responses from all stages
|    |--> Provide Final Answer to User via **Streamlit Interface**
|
|--> **End: YouTube RAG Application Process Completed**
