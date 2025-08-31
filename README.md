VisionGuard AI – Privacy-Preserving Deidentification
🔒 Overview

VisionGuard AI is an open-source privacy-preserving deidentification tool that automatically redacts Personally Identifiable Information (PII) from both text and visual data.
It combines OCR, NLP, Computer Vision, and Layout-aware AI to anonymize documents such as healthcare records, ID cards, and financial forms — protecting privacy while maintaining data utility.

✨ Features

📄 OCR + NLP Layer → Extract text and detect PII (names, addresses, phone numbers, IDs).

👁 Vision Layer → Detect and redact faces, photos, stamps, and signatures.

📑 Layout-Aware Models → Handle complex forms and semi-structured documents.

🖊 Redaction & Export → Blur, mask, or replace sensitive info in original format (PDF → Redacted PDF).

⚡ Integration → CLI and REST API for real-world workflows.


Architecture

Pipeline Flow:Input Document → OCR + NLP → Vision Detection → Layout Understanding → Redaction & Export → Redacted Output
Tech Stack

OCR → Tesseract, EasyOCR

NLP → SpaCy, HuggingFace Transformers

Vision → YOLOv8, Detectron2, OpenCV

Layout-Aware Models → LayoutLMv3

Backend → Python, FastAPI, Flask

Deployment → Docker

Docs → Pandas, PyMuPDF, PDFPlumber


Installation & Usage
1. Clone Repo
git clone https://github.com/<your-username>/VisionGuard-AI.git
cd VisionGuard-AI

2. Install Dependencies
pip install -r requirements.txt

3. Run Redaction Tool
python src/redact.py samples/input.pdf --output samples/output_redacted.pdf

📊 Applications

🏥 Healthcare → Anonymizing patient medical records.

🏛 Governance → Redacting voter IDs, passports, legal docs.

💳 Fintech → Protecting KYC and compliance documents.

🏢 Enterprise → Automating bulk document redaction.

🔮 Roadmap

🌍 Multilingual support

✍️ Handwriting recognition

🌐 Web dashboard for non-tech users

🤝 Community contributions for open-source growth

🤝 Contributing

Contributions are welcome! Please fork this repo and submit pull requests.

📜 License

This project is licensed under the MIT License.

