# 🎥 Clip2Text – Transform Video Captions into Smart Summaries

Clip2Text is a **Streamlit-based web application** that extracts **YouTube captions (manual and auto-generated)** and converts them into **structured summaries** using the **Groq LLM API**.

The application also provides **live workflow logs**, **video thumbnail previews**, and **downloadable summary and transcript files** for a seamless user experience.

---

## ✨ Key Features

- **YouTube Caption Extraction**
  - Fetches subtitles using **yt-dlp**
  - Supports both **manual** and **auto-generated** captions

- **Transcript Processing**
  - Cleans and de-duplicates subtitle text for improved summarization

- **Multiple Summary Styles (Groq-powered)**
  - Short & Crisp
  - Detailed Notes
  - Study Notes
  - Job Interview Takeaways
  - Executive Brief

- **Live Workflow Logs**
  - Displays real-time processing logs for better transparency and debugging

- **Downloadable Results**
  - Export summary as `.txt`
  - Export transcript as `.txt`

---

## 🧰 Tech Stack

- **Frontend + Backend:** Streamlit
- **Captions Extraction:** `yt-dlp`
- **Text Processing:** Python
- **Summarization:** Groq API (`llama-3.1-8b-instant`)
- **Deployment:** Streamlit Community Cloud

---

## 📁 Project Structure

```text
Clip_2_Text/
├── app.py
├── requirements.txt
└── README.md
```

---

## 🧪 Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/SravyaSala/Clip_2_Text.git
cd Clip_2_Text/
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Add Your Groq API Key

Create a `.env` file in the project directory:

```env
GROQ_KEY=YOUR_GROQ_API_KEY
```

### 4. Run the Application

```bash
streamlit run app.py
```

Open your browser and visit:

```text
http://localhost:8501
```
