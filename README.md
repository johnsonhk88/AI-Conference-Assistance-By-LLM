# AI-Conference-Assistance-By-LLM


### Introdctions
#### Business/ Use case 
We often attend a lot of conference every day. We need take note for memory the key topic and leu 0content of this conversion and ensure we can take further action/activity following up the conference especially in business conference. After that,  We need spent a lot of the time to organize and write back into mintues, the send to all attendee for review and take further  . It is taking a lot of time.

This project intended to be used LLM Model for the purpose of assisting the user take conference note and record with speech convert into text context of these documents and faster to generate summary conference content and action item into text document, allow automatic send document to specific user the attend . 


### Technology use in this project
1. Automatic Speech Recognition (ASR) model
- converted the speech to text with support multilingual languages (Chinsese), auto language detection (openai)

2. Speaker identification model
- for classification which speaker to speak with speech 

3. LLM Model 
- try to use different open LLM models (e.g. LLama3, gemma 2) , prefer use local open LLM models(planning inference LLM model at offline in local machine)

4. retrieval augmented generation (RAG) with langChain  
- using training dataset for improvement the Text summaration task for conference speakers
- using Advance RAG technique improve retrieval accuracy (e.g. re-ranking, query extensions, auto-merging)

5. LoRA fine tuning model
- comparing RAG and fine tuning with LoRA performance (response time, token size, GPU Memory usage, accurary)


6. LLM Model evaluation
- use truLens or W&B framework for evaluation and debug LLM performance
- LLM evaluation : Content relevance, Answer Relevance, accuary, recall, precision 

7. AI agent
- use AI agent automatically trigger multiple function 

8. VectorDB 
- use Vector DataBase to store the converted Document context into embedding vector
- use Vector Database can find document similarity 

9. SQL Database
- use to store the conference record
- use for query history conference record

10. FrontEnd UI
- first version will be used Streamlit for Frontend UI
- later versions will be Full stack with Backend Restful API



### Installation and Setup
1. use requirements.txt for installation package dependencies
2. you can setup virual environment by venv 
3. add your google api key to .env file  for enviroment variables 

### Run Application
1. running ai-conference-dev.ipynb for develop the application
