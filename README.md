# ai-pdf-summary_&_tag-workflow
# 🧠 AI-Powered PDF Summarizer using n8n + Langchain + Google Gemini

This project is a local **n8n workflow** that automates the process of summarizing PDF documents using AI. It extracts content from a PDF stored on Google Drive, uses a Langchain agent powered by Google Gemini to generate a summary and tags, and appends the results into a Google Sheet.

---

## 🚀 Features

- ✅ Downloads PDF from Google Drive
- ✅ Extracts raw text content from the PDF
- ✅ Uses Google Gemini + Langchain to summarize the document
- ✅ Generates relevant tags from content
- ✅ Appends summary and tags to Google Sheets

---

## 🛠 Tech Stack

- [n8n](https://n8n.io/) (self-hosted)
- Langchain Agent
- Google Gemini (PaLM) - `gemini-2.0-flash` model
- Google Drive API
- Google Sheets API

---

## 🔁 Workflow Overview

1. **Manual Trigger** – Start the workflow with a click.
2. **Download PDF** – Pulls the file from Google Drive using file ID.
3. **Extract Text** – Extracts readable text from the PDF.
4. **AI Agent** – Sends content to Langchain Agent using Gemini model.
5. **Parse Response** – Splits the output into summary and tags.
6. **Append to Google Sheets** – Logs the result into a pre-linked Sheet.


---

## 📥 How to Use

1. Set up [n8n](https://docs.n8n.io/getting-started/installation/) on your local system.
2. Import `ai-pdf-summary-workflow.json` in the n8n editor.
3. Add the following credentials:
   - Google Drive OAuth2
   - Google Sheets OAuth2
   - Langchain agent using Gemini model (`gemini-2.0-flash`)
4. Create a Google Sheet with columns: `TAGS` and `SUMMARY`.
5. Run the workflow manually to test.

> **Note:** This version only supports **PDF files**.

---

## 🧠 Future Improvements

- Add support for DOCX, TXT, and image files
- Create a public UI using Streamlit or Gradio
- Add Slack/Email notifications on execution
- Error handling & logging

---

## 👤 Author

**Ankur Ghosh**  
🎓 B.Sc. (Hons) in Computer Science (AIML)  
🔗 [LinkedIn](https://www.linkedin.com/in/ankur-ghosh-344948246/)  
📬 Contact: ankurghosh@email.com 

---

## 🏷️ Tags

n8n, langchain, pdf summarizer, google gemini, google drive, google sheets, ai automation, document processing
