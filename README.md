An AI-powered application that generates personalized job application emails using job descriptions and candidate profiles.
Built with LangChain, Groq (ChatGroq), ChromaDB, and Streamlit for fast, high-quality email generation.

Features:

Generate professional job application emails
Uses LLMs via Groq Cloud (ChatGroq)
Context-aware generation using ChromaDB vector store
Matches resume/profile content with job descriptions
Fast inference with Groq’s high-performance models
Simple and interactive Streamlit UI

| Component       | Technology |
| --------------- | ---------- |
| UI              | Streamlit  |
| LLM Framework   | LangChain  |
| LLM Provider    | Groq Cloud |
| Model Interface | ChatGroq   |
| Vector Database | ChromaDB   |
| Language        | Python     |


job-applier-email-generator/
│
├── app/
│   ├── main.py              # Streamlit app entry point
│   ├── chains.py            # LangChain chains and prompts
│   ├── utils.py             # Helper utilities
│   ├── portfolio.py         # Load portfolio files
│
├── resource/
│   ├── portfolio.csv/             # portfolio data

│
├── vectorstore/               # ChromaDB persistent storage
│
├── .env                     # Environment variables
├── requirements.txt
└── README.md





Prerequisites:
Python 3.10+
Groq Cloud API Key
Virtual environment (recommended)


Environment Variables:
Create a .env file in the project root:
GROQ_API_KEY=your_groq_api_key_here

Installation:
Clone the repository

Create & activate virtual environment:
python -m venv venv
source venv/bin/activate   # Linux / macOS
venv\Scripts\activate      # Windows

Install dependencies:
pip install -r requirements.txt

Running the Application:
streamlit run app/main.py


The app will be available at:
http://localhost:8501


Contributing
Contributions are welcome!
Fork the repo
Create a feature branch
Commit changes
Open a Pull Request


License
This project is licensed under the MIT License.



Support
If you face issues or have feature requests, feel free to open an issue or reach out.
Happy coding!

