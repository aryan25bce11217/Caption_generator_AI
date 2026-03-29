# Caption Crafter AI
I have created a small Flask web app that helps users to generate short Instagram captions using Google Gemini.The user is able to enter description of his/her post and choose a mood, and the app generates a short caption for them.

 **Live Demo:**  
https://caption-crafter-ai-1.onrender.com/

## Features

* This project uses clean and modern UI
* I have tried to create a One-click caption generation
* I hve used the Gemini gemini-2.0-flash REST endpoint
* This project works locally and on cloud platforms
* I have deployed this for Render, Railway

## How it works

1. The user will submit a description and select the mood.
2. The backend side sends a short prompt to the Gemini API.
3. The app calls:
   `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent`
4. The project  model returns a caption.  
5. The app finally displays one clean line of text.

## Installation

Install the required packages:

```
pip install flask requests python-dotenv
```
## Running the app

Start the server:

```
python app.py
```

Open the app in your browser:

```
http://localhost:5000
```


##  Project structure  
```
/
│ app.py
│ requirements.txt
│ runtime.txt
│ Procfile
│ README.md
│ DEPLOYMENT.md
│ .gitignore
│
└── templates/
    └── index.html
```

##  Deployment  
I have created a fuul guide on how to deploy this project and it is mentioned in `DEPLOYMENT.md`.

## Future improvements

* Separate Gemini client module can be an important change
* Stronger rate limiting 
* Optional authentication might be helpful for users before generating captions
