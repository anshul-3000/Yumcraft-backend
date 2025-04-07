# 🍳 Yumcraft Backend

This is the backend API for **Yumcraft**, a recipe recommendation app powered by ingredient-based search and machine learning. Built with Flask and integrated with a recommendation model, it helps users discover recipes based on the ingredients they have.

---

## 🚀 Features

- Ingredient-based recipe recommendation using cosine similarity
- Clean and structured Flask API with CORS support
- Loads pre-trained recipe model and dataset
- Returns top matching recipes including name, ingredients, and image

---

## 📁 Project Structure
yumcraft-backend/ 
├── main.py # Flask app entry point 
├── route.py # API routes and recommendation logic 
├── models/ │ └── recipe_recommendation_model.pkl 
├── data/ 
    └── processed/ 
    └── recipes_processed.csv 
├── requirements.txt 
├── .gitignore 
└── README.md


---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Yumcraft-backend.git
cd Yumcraft-backend
