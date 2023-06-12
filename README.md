# VNRVJIET-Chatbot

**This chatbot answers queries related to VNRVJIET, it was built using Pinecone Vector Database, GPT 3.5 and Langchain**

### Live-Link - [app](https://askvnrvjiet.streamlit.app/)

### How to Use
simply head over to the app, and start chatting. it will answer questions that it was trained on.
you can also maintain a chat history, until U close the app.

Note that you also get the preview of the refined query.
![image](https://github.com/Userfound404/VNRVJIET-Chatbot/assets/97509220/0f0e0690-2b18-4fd7-ac09-d93a22070c95)


### Technical Details
- Frontend: streamlit
- Backend: OpenAI api, sentence-transformers
- Database: Pinecone P1 storage

### Cloning and Making Changes
To clone this project, follow these steps:

Clone this repository using the following command:

1. `git clone https://github.com/Userfound404/VNRVJIET-Chatbot.git`
2. Install the necessary dependencies: `pip install -r requirements.txt`
3. Run the Streamlit app:
`streamlit run app.py`
4. Make changes to the code and push them to your own repository. To push your changes to your repository, use the following command:
`git push origin master`

  
**make sure to update your API keys in `utils.py` and `app.py`**
