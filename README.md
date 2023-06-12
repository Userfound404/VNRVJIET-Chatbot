# VNRVJIET-Chatbot

**This chatbot answers queries related to VNRVJIET, it was built using Pinecone Vector Database, GPT 3.5 and Langchain**

### Live-Link - [app](https://askvnrvjiet.streamlit.app/)
### blog - [here](https://medium.com/@swheatdreamz/how-chatgpt-took-chatbots-to-a-new-realm-28e0c7459502)

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

### Working
![image](https://github.com/Userfound404/VNRVJIET-Chatbot/assets/97509220/b35edb6f-7f5d-4011-b486-075fd1ecc2cc)

The image above show exactly how our application can be created. We divide our data into chunks and utilise text embedding to store distinct vectors in a database. Now, whenever a user enters a query, the text embedding is used to retrieve the closest datapoint. Our LLM specialises in comprehending context, including earlier conversations. The model then returns the relevant database answer.
Remember we're not exactly changing the architecture of the model for fine-tuning but are leveraging the contextual understanding of the LLM.

read more in my blog.
