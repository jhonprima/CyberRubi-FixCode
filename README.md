"# CyberRubi-FixCode" 
# 🦊 Cyberfox – Chatbot Edukatif Keamanan Siber untuk Anak

**Cyberfox** adalah chatbot AI edukatif yang dirancang untuk membantu anak-anak memahami dasar-dasar keamanan siber secara interaktif dan ramah anak. Proyek ini menggunakan arsitektur Retrieval-Augmented Generation (RAG) dengan teknologi modern seperti:

- ⚛️ React.js (Frontend)
- 🧠 Cohere AI (Model Bahasa)
- 🌐 Node.js + Express (Backend API)
- 🗃️ PostgreSQL + PgVector (Database & Vector Store)
- 🧩 LangChain (Processing & Retrieval Layer)

---

## 📁 Struktur Proyek

├── backend/ # Backend Express.js
├── frontend/ # Frontend React (Vite)
├── backend-langchain/ # Engine LangChain + Cohere + Vector DB
├── .env # Konfigurasi rahasia (API key, DB, dll)


---

## 🚀 Fitur Utama

- Edukasi keamanan siber untuk anak dengan bahasa sederhana
- Menjawab pertanyaan berdasarkan dokumen terkurasi (RAG)
- Penyimpanan histori chat per pengguna
- Proses embedding & pencarian vektor dengan LangChain + PgVector
- Integrasi Cohere AI sebagai model LLM

---

## ⚙️ Instalasi & Konfigurasi

### 1. Clone Repository
```bash
git clone https://github.com/jhonprima/CyberRubi-Fixcode.git
cd CyberRubi

Setup Frontend (React + Vite)
cd frontend
pnpm install         # atau npm install
pnpm dev             # jalankan frontend di localhost:5173


Setup Backend API (Node.js + Express)
bash
Copy
Edit
cd ../backend
pnpm install
pnpm dev             # jalankan backend di localhost:3000


.ENV
PORT=3000
LANGCHAIN_BACKEND_URL=http://localhost:8000
COHERE_API_KEY=your_cohere_api_key
DB_URL=postgresql+psycopg2://user:password@localhost:5432/cyberfox
 Setup LangChain + Cohere + PgVector (Python)
bash
Copy
Edit
cd ../backend-langchain
python -m venv venv
source venv/bin/activate  # gunakan `venv\Scripts\activate` di Windows
pip install -r requirements.txt
uvicorn main:app --reload --port 8000




ARSITEKTUR SEDERHANA
User ↔ React Frontend ↔ Express Backend ↔ LangChain RAG ↔ Cohere + Pinecone

 Contoh Prompt


"Apa itu password yang aman?"
→ Cyberfox menjelaskan pentingnya kombinasi huruf, angka, dan simbol.






