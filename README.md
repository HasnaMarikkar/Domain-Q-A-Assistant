# 🤖 Domain-Restricted Q&A Assistant

Domain-Restricted Q&A Assistant is a Streamlit-based AI application that answers questions only within a selected domain using a custom CSV knowledge base. The app combines OpenAI’s GPT models with domain restrictions and personalized response styles to create a focused AI assistant experience.

---

## 🛠️ Technologies Used

* Python
* Streamlit
* Pandas
* OpenAI API
* CSV-based Knowledge Base

---

## 🚀 Features

* Domain-specific AI assistant
* CSV knowledge base upload system
* AI responses powered by OpenAI
* Domain restriction enforcement
* Adjustable response styles:

  * Tone
  * Length
  * Audience level
* Quick prebuilt questions
* Session state persistence
* Error handling for invalid uploads and API issues
* Simple and responsive Streamlit UI

---

## ⚙️ Process

User selects a domain from the Setup tab

User uploads a CSV knowledge base containing:

* `topic`
* `information`

The application:

* Loads and validates the CSV
* Converts the CSV into a formatted knowledge base
* Stores it in Streamlit session state

User enters:

* A question
* Tone preference
* Response length
* Audience level

The app:

* Builds a structured prompt
* Sends it to OpenAI GPT-4o-mini
* Displays the AI-generated answer

Users can also select quick template questions from the Quick Questions tab.

---

## 🧑‍💻 How I Built It

I built this project using Streamlit as the frontend framework and OpenAI’s API for AI-generated responses.

The development process involved:

* Designing a multi-tab Streamlit interface
* Creating domain-restricted prompt engineering
* Building CSV upload and validation functionality
* Managing persistent state using Streamlit session state
* Integrating OpenAI API calls
* Adding customizable response styles
* Creating reusable helper functions
* Implementing quick-question templates
* Handling file and API errors gracefully

---

## 📚 What I Learned

* How Streamlit session state works
* Working with CSV uploads in Streamlit
* Prompt engineering for domain restriction
* Integrating OpenAI APIs into Python applications
* Structuring reusable functions and clean app architecture
* Error handling for file uploads and API responses
* Building multi-tab interactive applications
* Managing dynamic UI components in Streamlit

---

## 📈 Overall Growth

This project improved my understanding of AI application development, prompt engineering, and frontend-backend interaction using Streamlit.

It also helped me practice:

* Clean function-based architecture
* API integration
* State management
* User-focused UI design
* Building domain-constrained AI systems

---

## 🔧 What Could Be Improved

* Add conversation history
* Support multiple uploaded knowledge bases
* Add embeddings/vector search for smarter retrieval
* Improve prompt engineering
* Add authentication system
* Export chat responses
* Add dark mode support
* Improve UI styling and animations
* Add real-time streaming responses

---

## ▶️ How to Run It

```bash
git clone <your-repo-url>
cd domain-qa-assistant
pip install -r requirements.txt
streamlit run app.py
```

Then open:

```bash
http://localhost:8501
```

---

## 📂 Required CSV Format

Example CSV structure:

```csv
topic,information
Protein,Protein helps build muscle.
Cardio,Cardio improves heart health.
Budgeting,Budgeting helps manage expenses.
```

Required columns:

* `topic`
* `information`

---

## 🔑 API Setup

Enter your OpenAI API key in the sidebar after launching the application.

Get your API key from:

[OpenAI Platform](https://platform.openai.com/api-keys?utm_source=chatgpt.com)
