Markdown
# 🌾 AgroGuard
> **AI-Driven Smart Farming & Crop Protection System**

![Project Status](https://img.shields.io/badge/Status-Active-success?style=flat-square)
![Python](https://img.shields.io/badge/Python-3.9+-blue?style=flat-square&logo=python)
![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=flat-square&logo=fastapi)
![AI](https://img.shields.io/badge/AI-Gemini%203%20Flash%20preview-orange?style=flat-square&logo=google)
![Groq](https://img.shields.io/badge/AI_Chatbot-Groq%20Llama%203.1-f55036?style=flat-square)
![Multilingual](https://img.shields.io/badge/Multilingual-5%20Languages-9C27B0?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)

---

## 📖 About The Project

**AgroGuard** is an innovative agricultural management platform designed to empower modern farmers with real-time insights and automated security. Acting as a digital sentinel for your farmland, AgroGuard leverages **Generative AI** and **Machine Learning** to monitor crop health, predict spoilage risks, optimize soil usage, and forecast market prices. 

With our latest update, AgroGuard breaks language barriers, offering a fully localized experience to ensure every farmer gets access to cutting-edge technology in the language they understand best.

---

## ✨ Key Features & Recent Updates

### 🌍 **Seamless Multilingual Support (NEW)**
AgroGuard is now fully accessible in **5 languages**: English, Hindi (हिंदी), Marathi (मराठी), Odia (ଓଡ଼ିଆ), and Telugu (తెలుగు).
* **Dynamic UI Translation:** Instantly switch languages across the entire frontend (HTML/JS) via the top navigation bar.
* **Localized AI Responses:** The backend Gemini AI integration natively processes and generates farming plans, spoilage advice, and market predictions in your preferred language.
* **Smart Language Caching:** Backend memory optimized with language-specific cache keys for ultra-fast query loading.

### 🤖 1. AI Crop Planner (`crop_planner.html` / `ai_agent_api.py`)
* **Intelligent Rotation:** Generates optimal crop rotation plans based on soil type, season, and previous harvest.
* **Data Visualization:** Renders interactive charts powered by `Chart.js` and clean Markdown outputs via `Marked.js`.

### 📉 2. Spoilage & Logistics Predictor (`predict.html` / `spoilage_api.py`)
* **Store vs. Sell Analysis:** Recommends whether to store crops or sell them immediately based on real-time temperature, humidity, and transit times.
* **Risk Scoring:** Assigns a "Spoilage Risk Score" to help mitigate losses.

### 💰 3. Market Price Forecaster (`price_prediction.html` / `price_api.py`)
* **Profit Estimation:** Accurately forecasts potential selling prices, calculating base costs and predicting ROI.
* **Market Mapping:** Provides data-driven recommendations on top nearby hubs and local/export market levels.

### 💬 4. Groq-Powered AI Assistant (NEW)
* **Instant Answers:** A lightning-fast, floating chatbot available on every page, powered by Groq's `llama-3.1-8b-instant` model.
* **Context-Aware & Multilingual:** Automatically detects the language selected in your UI and replies natively in that language.
* **Optimized Advice:** Specifically tuned to deliver highly concise, bulleted responses to save farmers time and minimize token usage.

---

## 📂 Folder Structure

The project has been organized to cleanly separate the frontend UI from the backend AI logic:

```text
AgroGuard/
├── backend/
│   ├── main.py                 # FastAPI application entry point & CORS configuration
│   ├── ai_agent_api.py         # AI Crop Planner & Rotation Logic
│   ├── chatbot_api.py          # Groq-Powered AI Chatbot Logic
│   ├── price_api.py            # Market Price & Profit Prediction AI
│   └── spoilage_api.py         # Storage/Logistics Risk Evaluation AI
│
├── frontend/
│   ├── index.html              # Main Landing Page
│   ├── about.html              # About Us & Platform Information
│   ├── crop_planner.html       # AI Crop Planning Dashboard
│   ├── predict.html            # Spoilage & Logistics Predictor Dashboard
│   ├── price_prediction.html   # Market Price & Profitability Dashboard
│   └── assets/                 # CSS stylesheets and images (e.g., style.css, logo.png)
│
├── .env                        # Environment variables (API Keys)
└── README.md                   # Project documentation
```


## 🚀 Getting Started

Follow these steps to set up the project locally.

### Prerequisites
* Python 3.9 or higher
* A Google Cloud API Key (for Gemini)

### Installation

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/Anandprasad03/AgroGuard.git](https://github.com/Anandprasad03/AgroGuard.git)
    cd AgroGuard
    ```

2.  **Install Dependencies**
    ```bash
    pip install fastapi uvicorn requests python-dotenv pydantic
    ```

3.  **Configure Environment**
    Create a `.env` file in the root directory `AgroGuard/` and add your API key:
    ```env
    GEMINI_API_KEY=your_google_api_key_here
    GROQ_API_KEY=your_groq_api_key_here
    ```

4.  **Run the Backend**
    ```bash
    uvicorn backend.main:app --reload
    ```
    *(Note: The server will run on `https://agrogaurd-1.onrender.com`)*

5.  **Launch the App**
    Simply open `frontend/index.html` in your web browser to access the dashboard.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  **Fork** the Project
2.  **Create** your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  **Commit** your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  **Push** to the Branch (`git push origin feature/AmazingFeature`)
5.  **Open** a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p align="center">
  <i>Built with ❤️ for sustainable farming.</i>
</p>