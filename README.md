
# SQL to ER Diagram Generator (Crow's Foot Notation)

A web-based tool that uses AI to automatically generate high-quality, downloadable Entity-Relationship Diagrams (ERDs) from SQL Data Definition Language (DDL) statements.

This project leverages the **Google Gemini API** to parse and understand SQL schemas, and renders them visually in the industry-standard **Crow's Foot notation** using **Mermaid.js**.


---

## 🚀 Features

- **AI-Powered Analysis:**  
  Intelligently parses SQL `CREATE TABLE` statements, including columns, data types, primary keys, and foreign keys.

- **Crow's Foot Notation:**  
  Renders clean and professional ER diagrams using the widely adopted Crow’s Foot notation.

- **High-Quality Exports:**  
  Download your diagrams in various formats suitable for documentation, presentations, or collaboration:
  - **PNG** – High-resolution raster image  
  - **JPEG** – Standard quality image  
  - **PDF** – Portable document format  
  - **SVG** – Scalable vector graphic for infinite zoom and clarity

- **Responsive UI:**  
  A clean, modern, and intuitive web interface.

- **Lightweight Backend:**  
  Powered by Flask, ensuring fast performance and minimal setup.

---

## 🧰 Technology Stack

### 🔧 Backend
- Python 3
- Flask (for web server and API)
- Google Gemini API (for SQL analysis)
- python-dotenv (for environment variable management)

### 🌐 Frontend
- HTML5
- CSS3
- Vanilla JavaScript
- Mermaid.js (for rendering diagrams)
- jsPDF (for PDF export functionality)

---

## ⚙️ Setup and Installation

Follow these steps to run the project locally:

### 1. Prerequisites

- [Python 3.10+](https://www.python.org/downloads/)
- `pip` (Python package manager)
- A **Google Gemini API Key** (get it from [Google AI Studio](https://aistudio.google.com/app/apikey))

---

### 2. Clone the Repository

```bash
git clone https://github.com/your-username/sql-to-erd.git  # Replace with your GitHub repo URL
cd sql-to-erd
```

---

### 3. Create and Activate a Virtual Environment

**macOS / Linux:**

```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows:**

```cmd
python -m venv venv
venv\Scripts\activate
```

---

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 5. Configure Environment Variables

Create a `.env` file in the root directory of the project:

```env
# .env
GEMINI_API_KEY="your_actual_api_key_goes_here"
```

> **Note:** Replace `"your_actual_api_key_goes_here"` with the actual API key from Google AI Studio.

---

### 6. Run the Application

```bash
python app.py
```

Visit: [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.

---

## 📝 How to Use

1. Open the application in your browser.
2. Paste your SQL `CREATE TABLE` statements into the input box (use the placeholder as a guide).
3. Click the **"Generate Diagram"** button.
4. The generated ER diagram will appear below.
5. Use the download buttons to save the diagram as PNG, JPEG, PDF, or SVG.

---

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

---

## 🙏 Acknowledgements

- **Google Gemini** – For the AI engine powering SQL parsing  
- **Mermaid.js** – For diagram rendering  
- **Flask** – For the web application framework  
