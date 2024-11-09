**Start: YouTube RAG Application**

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
|--> **Final Output Generation**
|    |
|    |--> TXT files containing transcripts are ready for use
|
|--> **End: YouTube RAG Application Process Completed**
