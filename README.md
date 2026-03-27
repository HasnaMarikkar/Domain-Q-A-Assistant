# Domain-Q-A-Assistant
Streamlit Web Application

An AI assistant that answers questions within a chosen domain, using your own CSV as a knowledge base.
Install & Run
bashpip install streamlit pandas openai
streamlit run app.py
How to Use

Setup tab — pick a domain and upload your CSV
Sidebar — paste your OpenAI API key
Chat tab — ask a question and hit Get Answer
Quick Questions tab — click a pre-built question to fill the chat

CSV Format
Your file must have two columns: topic and information
csvtopic,information
Hydration,Drink at least 8 cups of water per day.
Sleep,Adults need 7–9 hours of sleep for optimal recovery.
Domains
Fitness · Travel · Biology · Personal Finance
