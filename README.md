# 🧿  Eye Disease Assistant – OCT Image & Medical Chatbot

An AI-powered eye disease assistant that analyzes Retinal OCT images and provides clear, structured explanations using a medical knowledge-based chatbot.
This project is designed for educational and assistive purposes only.

**🔍 What This Bot Does**

Accepts Retinal OCT images uploaded by the user

Uses a deep learning model to predict eye conditions:

CNV

DME

DRUSEN

NORMAL

Provides a confidence score for the prediction

Explains the condition using a medical knowledge-based chatbot (RAG)

Displays both the uploaded image and the chatbot response in a single interface

⚠️ This system does not provide medical diagnosis or treatment advice.

**🛠️ Technologies Used**

TensorFlow / Keras – model inference

Flask – backend server

LangChain – chatbot orchestration

Pinecone – vector database for medical knowledge

Gemini API – language model

HTML / CSS / JavaScript – chatbot interface

**📁 Project Structure**
Eye_Disease_Chatbot/
│
├── app.py                  # Flask application
├── src/
│   ├── model.py             # Model loading & prediction logic
│   ├── helper.py            # Embeddings and utility functions
│   ├── prompt.py            # System prompt
│
├── templates/
│   └── chat.html            # Chatbot UI
│
├── static/
│   └── style.css            # UI styling
│
├── eye_diseases_weights.weights.h5   # Model weights
├── .env                     # API keys
├── requirements.txt
└── README.md

****⚙️ Setup Instructions****
1️⃣ Clone the repository
git clone <your-github-repo-link>
cd Eye_Disease_Chatbot

2️⃣ Create and activate a virtual environment
python -m venv medchatenv
source medchatenv/bin/activate   # Linux / Mac
# medchatenv\Scripts\activate    # Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Configure environment variables

Create a .env file in the root directory:

PINECONE_API_KEY=your_pinecone_api_key
GOOGLE_API_KEY=your_gemini_api_key

5️⃣ Run the application
python app.py


The app will start at:

http://127.0.0.1:8080

****🧑‍⚕️ How to Use the Bot****
**🔹 Text-Based Questions**

Open the chatbot interface

Type your question related to eye diseases

The chatbot responds using medical knowledge

**🔹 OCT Image Analysis**

Click the upload icon

Select a Retinal OCT image

The system:

Displays the uploaded image

Predicts the eye condition

Shows the confidence score

Provides a structured explanation

**⚠️ Important Disclaimer
**
This project is for educational and assistive purposes only.
It is not a diagnostic tool and should not be used for medical decisions.

Always consult a qualified eye-care professional for diagnosis and treatment.
