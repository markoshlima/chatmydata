# **Introduction**

This project is about to create a chat interface to "talk" with your data using Large Language Model (LLM). The objective is create a channel with Lang Chain to read structured data like JSON, and then with ChatGPT get the answer for the user question.

# **Project**

The project is based in an Angular frontend that do the interface for the user, and a Python backend to read the data and create chain with LangChain for finally integrate with ChatGPT.

![alt text](https://raw.githubusercontent.com/markoshlima/chatmydata/main/docs/diagram.png)

In this project there is a Json file with some basic structured data:
```
{
	"name":"string",
	"age": "integer"
}
```
After that is possible to get information from the structured data using natural language, like: "Who is the oldest?", and the chat answer: "The oldest person is ...".
The next image shows the results of some conversation:

![alt text](https://github.com/markoshlima/chatmydata/blob/main/docs/front-screen.png?raw=true)

Note that the model could understaind both english and portuguese language/question, and cold undersataind that it was talking about people, probably baause of metadata "age" and "name".

# Addition Information & Setup

-  To run the project change the chatmydata-back/constants.py,new file as the instructions inside it.
- Run ./bootstrap.sh
- Pre requisites for backend are:
	- Python 3.7.10
	- Flask 2.0.3
	- pip 20.2.2
	- pip install flask, openai
- To run frontend basicly install npm modules and execute ng serve
