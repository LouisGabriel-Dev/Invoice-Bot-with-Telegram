# Invoice-Bot-with-Telegram

An AI-powered Invoice Data Extractor and Automation System built on self-hosted infrastructure. This Telegram bot automatically processes incoming invoice documents (PDF/DOCX), extracts key financial information (Invoice Number, Date, Amount, Vendor, etc.) using AI, and instantly logs the structured data into Google Sheets for seamless expense tracking and bookkeeping.

## 🎥 Video Demo
<img width="400" alt="Invoice Extractor Bot Telegram Demo" src="https://github.com/user-attachments/assets/YOUR_VIDEO_OR_GIF_ASSET_ID" />

---

## 📝 Project Overview

### ⚠️ The Problem
Managing financial records manually from various suppliers or freelancers can be a major operational bottleneck:
* **Manual Data Entry:** Spending hours copying invoice numbers, dates, and line items from PDFs/docx into a company spreadsheet.
* **Human Error:** High risk of typos, missed digits, or miscalculated totals during manual data entry.
* **Delayed Bookkeeping:** Invoices get buried in chat histories or emails before they are logged, leading to inaccurate financial overviews.

### 💡 The Solution
This project automates the entire expense logging pipeline directly inside Telegram. By simply forwarding or uploading an existing invoice to the bot, the system will:
* **Automatically Parse & Extract Key Data:** Use LLM/AI vision capabilities to read invoice files and extract details like Invoice Number, Issue Date, Due Date, Total Amount, and Vendor Name.
* **Eliminate Manual Data Entry:** Instantly route and append the extracted, structured data into a designated **Google Sheets** spreadsheet in real-time.
* **Streamline Bookkeeping:** Keep financial records updated 24/7 with zero human intervention required for data transcription.

---

## 🛠️ Technical Specifications

### Tech Stack
* **Automation Engine:** n8n (Self-Hosted via Docker Compose)
* **Interface Platform:** Telegram Bot API (Receives document/image inputs)
* **OCR Engine:** OCR.space API (Performs Optical Character Recognition to extract raw text from PDFs)
* **AI Integration:** Gemini API / LLM Text Parser (Structures and refines raw OCR text into specific data points)
* **Spreadsheet Backend:** Google Sheets API (Data Destination)
