# LegalEase AI 📜✨

**An AI-powered legal assistant to demystify complex legal documents for the average Indian citizen.**


### [➡️ View Live Demo]([(https://sanjaykumar-nb.github.io/Legalease-AI/])

## The Problem

In India, the average citizen is frequently required to sign legal documents for renting a house, taking a loan, or starting a job. These documents are often filled with dense legal jargon, creating a significant **information asymmetry**. This knowledge gap puts individuals at a disadvantage, potentially leading them to agree to unfair terms, hidden clauses, and significant financial risks. Access to professional legal advice is often expensive and time-consuming, leaving many people feeling vulnerable and unempowered.

## The Solution

**LegalEase AI** is a free, web-based tool that leverages the power of Google's Gemini 1.5 Pro to bridge this gap. It acts as a personal AI legal analyst, transforming complex legal text into simple, actionable insights. By processing documents entirely in the user's browser, it ensures absolute privacy and builds trust. The application provides a multi-layered analysis, allowing users to understand their rights and obligations *before* they sign, thereby democratizing legal knowledge and promoting fairer agreements.

## 🚀 Key Features

* **Multi-Layered Analysis:** Goes beyond simple translation to provide:
    * 💰 **Financial Summary:** A clear breakdown of all financial commitments and projections.
    * 🔍 **Loopholes & Ambiguities:** Flags unclear or unfavorable clauses and explains the potential risks.
    * ✅ **Key Issues Summary:** Highlights the most critical obligations and terms.
    * ⚖️ **Legal Citations:** Cross-references clauses with relevant sections of Indian Law.
* **Interactive Q&A:** Users can ask specific questions about the document in plain English and get contextual answers.
* **Multilingual Support:** The entire analysis can be delivered in **English, Tamil (தமிழ்),** or **Hindi (हिन्दी)** to cater to a diverse user base.
* **Shareable PDF Report:** A one-click feature to generate a clean, printable summary of the AI's findings that users can save or share.
* **100% Privacy-First:** All PDF processing and analysis happens client-side. No documents are ever uploaded or stored on a server.

## 🛠️ Tech Stack

* **AI Engine:** Google Gemini 1.5 Pro API
* **Frontend:** Vanilla HTML5, CSS3, JavaScript (ES6+)
* **PDF Parsing:** PDF.js Library
* **Hosting:** GitHub Pages

## 🏛️ Architecture

LegalEase AI operates on a completely **serverless, client-side architecture**.

1.  The user uploads a PDF, which is read directly in the browser using **PDF.js**.
2.  The extracted text is sent along with a specialized, multi-persona prompt to the **Google Gemini API**.
3.  The API returns a structured JSON object containing the full analysis.
4.  The frontend JavaScript parses this JSON and dynamically displays the results.

This approach ensures maximum privacy and security, as the user's sensitive documents never leave their computer.

## ⚙️ How to Run Locally

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sanjaykumar-nb/genai.git](https://github.com/sanjaykumar-nb/genai.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd genai
    ```
3.  **Open `index.html`** in your web browser.

    *(Note: For local development, you will need to add your Google Gemini API key to the `script.js` file.)*

---
