Here’s a clean, professional **`README.md`** you can drop straight into your repo **`chumcred_pdf_to_word`**.

````markdown
# Chumcred PDF to Word Converter (OCR)

A Streamlit-based web application that converts PDF files (including scanned PDFs) into editable Microsoft Word documents using OCR (Optical Character Recognition).

This tool is designed for reliability on Windows and supports multi-page PDFs, configurable OCR settings, and direct download of `.docx` files.

---

## 🚀 Features

- Convert **scanned PDFs** and **image-based PDFs** to Word
- Supports **multi-page PDFs**
- OCR powered by **Tesseract**
- Adjustable **DPI** and **page segmentation modes**
- Simple **Streamlit UI**
- Download output as `.docx`
- Works fully **offline** once installed

---

## 🧱 Tech Stack

- **Python 3.10+**
- **Streamlit**
- **Tesseract OCR**
- **pdf2image**
- **Poppler (Windows)**
- **python-docx**
- **Pillow**

---

## 📂 Project Structure

```text
chumcred_pdf_to_word/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
````

---

## ⚙️ Installation (Windows)

### 1️⃣ Clone the repository

```bash
git clone https://github.com/<YOUR_USERNAME>/chumcred_pdf_to_word.git
cd chumcred_pdf_to_word
```

---

### 2️⃣ Create and activate virtual environment (recommended)

```bash
python -m venv .venv
.venv\Scripts\activate
```

---

### 3️⃣ Install Python dependencies

```bash
pip install -r requirements.txt
```

---

## 🔧 External Dependencies (Required)

### ✅ Install Tesseract OCR (Windows)

Download and install from:
[https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)

Default install path:

```text
C:\Program Files\Tesseract-OCR\tesseract.exe
```

---

### ✅ Install Poppler for Windows

Download Poppler binaries from:
[https://github.com/oschwartz10612/poppler-windows/releases](https://github.com/oschwartz10612/poppler-windows/releases)

Extract to:

```text
C:\Users\<YOUR_USERNAME>\poppler
```

Ensure the following file exists:

```text
C:\Users\<YOUR_USERNAME>\poppler\poppler-XX.XX.X\Library\bin\pdfinfo.exe
```

---

## ▶️ Running the App

```bash
streamlit run app.py
```

Open your browser at:

```
http://localhost:8501
```

---

## 📝 Usage

1. Upload a PDF file
2. Select OCR language and settings
3. Click **Convert to Word**
4. Download the generated `.docx` file

---

## 🛠 Troubleshooting

### ❌ `PDFInfoNotInstalledError`

* Poppler not installed correctly
* `pdfinfo.exe` not found
* Ensure correct `POPPLER_BIN` path in `app.py`

### ❌ `TesseractNotFoundError`

* Tesseract OCR not installed
* Incorrect `tesseract.exe` path
* Verify installation directory

---

## 🌍 Cross-Platform Notes

* The current configuration is optimized for **Windows**
* Linux/macOS users must install:

  * `poppler-utils`
  * `tesseract-ocr`
* Paths can be adapted using environment variables

---

## 📌 Roadmap (Optional Enhancements)

* Auto-detect searchable vs scanned PDFs
* Preserve tables and layout
* Batch PDF uploads
* Dockerized deployment
* Streamlit Cloud support

---

## 👤 Author

**Chumcred Limited**
AI • Data • Financial Analytics

---

## 📄 License

MIT License — free to use, modify, and distribute.

