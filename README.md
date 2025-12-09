# AI-powered-Company-broacher-
🧾 About the Project

The AI Powered Website Text Summarizer & Brochure Generator is a tool designed to automatically read, analyze, and summarize website content using LLM
The system intelligently extracts links, fetches relevant pages, processes the text, and generates a clean, readable summary or brochure using structured system prompts and user prompts.
This project demonstrates how AI can transform raw website data into meaningful, human-friendly content. Whether it's summarizing an article, generating a product brochure, or analyzing a company website, the tool provides an automated, privacy friendly, and fast workflow powered completely.

🛠 Tech Stack
🔹 Artificial Intelligence
OpenAI API (gpt-5-nano / gpt-4.1-mini) — For prompt-based text generation
Custom System & User Prompts — Controls summarization behavior and output style

🔹 Backend & Logic
Python — Main language for backend logic
BeautifulSoup- Extracts text from webpages
Requests — Fetches website content
JSON Processing — For structured communication with the model

🔹 Automation & Processing
Link Extraction Pipeline — Identifies relevant pages (About, Careers, etc.)
Content Fetching Workflow — Scrapes and cleans website tex
Prompt-Oriented Text Generation — Uses system + user prompts to generate summaries or brochures

🔹 Development Tools
Jupyter Notebook — Development and testing
dotenv — Secure API key management
IPython Markdown Display — Clean output formatting


          ┌─────────────────┐
          │   Input: URL    │
          └───────┬─────────┘
                  │
        ┌─────────▼───────────┐
        │   Web Scraper       │
        │ fetch_links()       │
        │ fetch_contents()    │
        └─────────┬───────────┘
                  │ scraped HTML/text
                  ▼
        ┌──────────────────────────┐
        │ GPT Link Selector Agent  │
        │  (gpt-5-nano)            │
        └───────┬──────────────────┘
                │ selected links
                ▼
     ┌──────────────────────────────┐
     │ Scraper fetches sub-pages    │
     └────────┬─────────────────────┘
              │ combined content
              ▼
     ┌──────────────────────────────┐
     │ GPT Brochure Generating Agent│
     │     (gpt-4.1-mini)           │
     └────────┬─────────────────────┘
              │ markdown brochure
              ▼
       ┌────────────────────┐
       │ Render to user     │
       │  Markdown output   │
       └────────────────────┘

