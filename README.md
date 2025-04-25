# 🌴 VacayFinder — AI-Powered Indian Vacation Recommendation App

VacayFinder is a Flask-based web application that recommends personalized travel destinations within India. Powered by the **Gemini API**, it uses AI to analyze uploaded vacation images, user preferences, and geographic data to suggest the perfect getaway — complete with itineraries, seasonal tips, and nearby options.

---

## ✨ Features

- 🧠 **AI Theme Detection**  
  Uses Google Gemini to classify vacation images into themes like beach, mountain, forest, urban, etc.

- 📍 **Smart Location Filtering**  
  Calculates distance between user's city and destinations using real lat/lon coordinates (Haversine formula via `geopy`)

- 🧭 **Season & Activity Matching**  
  Recommends places based on season, desired weather, activities, travel companions, and distance range

- 🗺️ **Curated Indian Dataset**  
  Custom JSON dataset of Indian destinations with location, theme, safety, budget, and image metadata

- 📬 **Contact Form with JSON Storage**  
  Stores user messages to a `contact_submissions.json` file on the backend

- 🔐 **Login / Signup Pages**  
  UI-ready pages for authentication with routing support (no backend auth yet)

---

## 🛠 Built With

- [Python 3.13](https://www.python.org/)
- [Flask](https://flask.palletsprojects.com/)
- [Google Generative AI (Gemini)](https://ai.google.dev/)
- [Geopy](https://geopy.readthedocs.io/)
- HTML, CSS, JavaScript
- Flask extensions: `flask-limiter`, `flask-caching`, `python-dotenv`

---

## 🗂 Project Structure

```
VacayFinder/
├── app.py
├── requirements.txt
├── myenv.env
├── contact_submissions.json
│
├── /templates
│   ├── index.html
│   ├── questions.html
│   ├── login_cleaned.html
│   └── signup_cleaned.html
│
├── /static
│   ├── styles.css
│   ├── script.js
│   └── /data
│       └── dataset.json
```

---

## 🚀 Getting Started

1. Clone the repository
2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```
3. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file and add your Gemini API key:
   ```
   GEMINI_API_KEY=your-gemini-api-key
   ```
5. Run the app:
   ```bash
   python app.py
   ```
6. Visit `http://127.0.0.1:5001` in your browser

---

## 📬 Contact

Built with ❤️ by Sreesh Jambulingam & Prazwal Ratti.  
Feel free to fork, contribute, or customize this for your own travel AI experiments!
