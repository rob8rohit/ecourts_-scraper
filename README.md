🏛️ eCourts Scraper (CLI + Flask API)
📘 Overview

This project allows users to fetch and check Indian eCourts case listings directly from the official eCourts portal
.
It supports both:

A Command-Line Interface (CLI) for developers and automation.

A Flask-based REST API for easy integration with web or mobile apps.

🚀 Features

✅ Fetch case details using CNR number or Case Type + Number + Year
✅ Check if the case is listed today or tomorrow
✅ Display serial number, date, and court name
✅ Optionally download case PDF if available
✅ Download entire cause list for a given day
✅ Store all results in structured JSON format
✅ Expose a Flask REST API for browser or Postman use

🧩 Project Structure
ecourts_scraper/
│
├── main.py                 # CLI entry point
├── app.py                  # Flask API interface
├── ecourt_client.py        # Core logic: data fetching and parsing
├── parsers.py              # HTML parsing helpers (BeautifulSoup)
├── utils.py                # Utility and file handling
├── requirements.txt        # Dependencies
├── data/                   # JSON results and PDFs
│   ├── case_result_YYYY-MM-DD.json
│   ├── cause_list_YYYY-MM-DD.json
│   └── pdf_YYYY-MM-DD_0.pdf
└── README.md
