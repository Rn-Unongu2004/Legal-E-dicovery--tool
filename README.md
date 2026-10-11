# Legal E-Discovery & Document Relevance Screening Tool

A beginner-friendly educational prototype for CSC 202. It processes a batch of TXT, PDF, and DOCX documents, searches user-selected keywords, calculates a keyword-match score, detects simple date/money/email patterns, records SHA-256 fingerprints, and exports a CSV report.

## Run locally
1. Install Python 3.10 or later.
2. Open a terminal in this folder.
3. Install dependencies: `pip install -r requirements.txt`
4. Start the app: `streamlit run app.py`
5. Open the local URL printed in the terminal.

## Test
Upload the `.txt` files in `sample_documents/`. Try keywords such as `contract, payment, delivery, breach, agreement`.

## Publish online (Streamlit Community Cloud)
1. Create a GitHub account and a new repository.
2. Upload `app.py`, `requirements.txt`, `README.md`, and optionally `sample_documents/`.
3. Sign in to Streamlit Community Cloud with GitHub.
4. Create a new app, select your repository and `app.py`, then deploy.
5. Copy the generated public URL for your lecturer.

The hosting service may change its interface or terms. Do not publish confidential case documents or credentials in the repository.

## Important limitations
- Keyword score is not a probability of legal relevance.
- This is not legal advice and does not decide admissibility.
- Scanned PDFs need OCR, which is not included.
- Human review remains essential.
- SHA-256 is a file fingerprint, not proof of authenticity.
