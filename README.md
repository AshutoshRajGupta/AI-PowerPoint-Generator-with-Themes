
# 📊 AI PowerPoint Generator with Themes

This project is an AI-powered PowerPoint presentation generator that automates the process of creating professional and engaging slides. Instead of spending hours manually writing content and designing layouts, users can simply enter a topic and let the system generate a complete PowerPoint file.

At its core, the project uses the Groq LLM (LLaMA-3.3-70B Versatile) to generate structured outlines, slide titles, and bullet points. The model ensures that the slides have a logical flow — starting from an introduction, moving into key points, applications, challenges, and ending with a conclusion.

To make presentations visually appealing, the project integrates with the Unsplash API for fetching high-quality, royalty-free images relevant to the topic. If the API is unavailable, it falls back to placeholder images to maintain slide consistency.

The design aspect is enhanced with a theme selector, allowing users to choose between Modern Blue, Classic Dark, and Minimal White themes. Each theme adjusts fonts, colors, and backgrounds to give a unique look and feel, much like real PowerPoint templates.

In short, this project combines the power of LLMs for content generation, python-pptx for presentation building, and Unsplash for visuals to deliver a fast, customizable, and professional presentation-making tool.

---

## 🚀 Features

* **AI-Powered Slide Content**

  * Uses **Groq LLM (LLaMA-3.3-70B Versatile)** for generating slide titles, bullet points, and structured outlines.
  * Automatically generates introductions, key points, challenges, and conclusions.

* **Theme Selector 🎨**

  * Choose from multiple pre-built themes:

    * Modern Blue
    * Classic Dark
    * Minimal White
  * Each theme customizes background colors, fonts, and text styles for a professional look.

* **Image Integration 🖼️**

  * Fetches high-quality images from **Unsplash API** using the slide's context.
  * Falls back to placeholder images if API key is not available.

* **Environment Variable Support 🔑**

  * API keys for Groq and Unsplash are securely stored in a `.env` file.
  * Eliminates the need to input keys manually every time.

* **Streamlit UI 🖥️**

  * Simple web interface for inputting topic, number of slides, and theme selection.
  * Click to generate and instantly download your PowerPoint.

---

## 🧠 Tech Stack

* **LLM**: [Groq LLaMA-3.3-70B Versatile](https://groq.com/)

  * Chosen for its **speed** and **efficiency** in text generation.
  * Provides structured, JSON-formatted content for slides.

* **Frontend**: [Streamlit](https://streamlit.io/)

  * Lightweight and easy-to-use UI framework.
  * Handles user inputs and displays download buttons.

* **Presentation Handling**: [python-pptx](https://python-pptx.readthedocs.io/)

  * Creates PowerPoint files programmatically.
  * Supports text formatting, themes, and images.

* **Image API**: [Unsplash API](https://unsplash.com/developers)

  * Provides free, high-quality stock images for slides.

* **Environment Management**: [python-dotenv](https://pypi.org/project/python-dotenv/)

  * Loads API keys from a `.env` file for security.

---

## 📂 Project Structure

```
📁 ppt_generator
│── main.py             # Streamlit app + PPT generator logic
│── .env                # API keys (not shared publicly)
│── requirements.txt    # Python dependencies
│── README.md           # Documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/ai-ppt-generator.git
cd ai-ppt-generator
```

### 2️⃣ Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Add your `.env` file

Create a file named `.env` in the root directory:

```env
GROQ_API_KEY='your_groq_api_key_here'
UNSPLASH_API_KEY='your_unsplash_api_key_here'
```

### 5️⃣ Run the Streamlit app

```bash
streamlit run main.py
```

---

## 🎯 How to Use

1. Enter a **topic** (e.g., "Artificial Intelligence in Education").
2. Select the **number of slides** (3–15).
3. Choose a **theme** (Modern Blue, Classic Dark, Minimal White).
4. Click **Generate Presentation**.
5. Download the `.pptx` file and open it in PowerPoint or Google Slides.

---

## 🔮 Future Enhancements

* **Realistic PowerPoint Templates** (beyond just background colors).
* **Custom slide prompts** (let users specify what slide 1, 2, or 3 should contain).
* **Image Style Selector** (Realistic, Illustration, Icon, Abstract).
* **Stable Diffusion / Hugging Face integration** for AI-generated images (instead of stock).
* **Preview Slides** before downloading.

---

## 🙌 Why This Project?

Creating engaging presentations manually is **time-consuming**.
This project automates the process by combining **LLMs for structured content** and **APIs for design elements**, producing a professional-quality presentation in seconds.

Perfect for:

* Students preparing projects 📚
* Professionals needing quick presentations 💼
* Educators creating teaching slides 👩‍🏫

---

## 📜 License

This project is open-source under the **MIT License**.

---

