
# ChatBot

A chatbot powered by an AI is that is designed to simulate human conversation, using natural language processing and machine learning techniques to understand and respond to user queries.


# Requirements:
Before you can run this chatbot locally, you need to have the following software installed on your system:

- Python 3.x  
- pip
- Git
# Installation :
To install the chatbot, follow these steps:

1. Clone or fork the repository:
```bash
git clone https://github.com/AGS2023/chatbt.git

```
\
2. Navigate to the cloned repository:
```bash
cd chatbt

```
\
3. Install the required dependencies:
```bash
pip install -r requirements.txt

```
\
4. Modify app.js to point to your local endpoint:
```js
fetch('https://localhost/predict')

``` 
\
5. Run the chatbot:
```bash
python app.py
```

# Deploying to Render:
To deploy this chatbot to Render, follow these steps:
1. Log in to Render using your GitHub account.

2. Create a new web service and import your repository.

\
3. Modify app.js to point to your Render endpoint:
```js
fetch('https://appname.onrender.com/predict')

```
\
4. Modify the build command in render to:
```bash
pip install -r requirements.txt

```
\
5. Modify the start command in render to:
```bash
start: "gunicorn app:app"

```
\
6. Push your changes to GitHub , Render will automatically build and deploy your chatbot.


# Usage:
Once the chatbot is running on Render, you can access it using the API endpoint at https://linktoyourapp.onrender.com. 

You can send text messages to the chatbot by sending a POST request to this endpoint with the following JSON payload or by using the graphical interface:

```json
{
    "message": "Hello, chatbot!"
}
```
\
The chatbot will respond with a JSON payload containing the chatbot's response to your message:
```json
{
    "response": "Hi there!"
}

```



