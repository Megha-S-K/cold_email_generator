# 📧 Cold Mail Generator
This project allows users to input the URL of a company's careers page. The tool then extracts job listings from that page and generates personalized cold emails. These emails include relevant portfolio links sourced from a vector database, based on the specific job descriptions.

## 🛠️ Tech Stack
- **Groq** – Utilized for high-performance ML model (llama 3.3)acceleration, enabling faster inference for large-scale text processing.
- **LangChain** – Used to orchestrate LLM workflows, chain prompts, and handle the end-to-end job extraction logic.
- **Streamlit** – Provides an interactive web interface for users to generate personalized cold emails with real-time previews.
- **ChromaDB** – Acts as a vector database for storing and retrieving job-related profile embeddings, allowing to attach profiles related to the reqirement.

## Architecture 

```bash
Career's Page ----> LLM --------> Extract jobs in json --------------->LLM----->Cold email
                            [job_title,skills,experience,           |
                                  job_description]                  |
                                        |                           |
                                        |                           |
                                        |                           |
                                  Vector store----------------------|
                                        
```




