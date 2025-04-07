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
- yumcraft-backend/ 
- ├── main.py # Flask app entry point 
- ├── route.py # API routes and recommendation logic 
- ├── models/ recipe_recommendation_model.pkl 
- ├── data/ processed/recipes_processed.csv 
- ├── requirements.txt 
- ├── .gitignore 
- └── README.md


---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Yumcraft-backend.git
cd Yumcraft-backend

python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

pip install -r requirements.txt

python main.py
```
- The app will run on http://localhost:5000

# 🧪 API Endpoint
## POST /recommend
```Request Body:
{
  "ingredients": ["onion", "tomato", "cheese"]
}
```
```Response:
[
  {
    "name": "Tomato Cheese Pasta",
    "ingredients": "tomato, cheese, pasta",
    "image_url": "https://example.com/image.jpg"
  },
  ...
]
```

# ☁️ Deployment (on Render)
- Push your project to GitHub

- Go to render.com

- Create a new Web Service

- Choose your GitHub repo

- Set:

     - Build Command: pip install -r requirements.txt

     - Start Command: python main.py

     - Environment: Python 3.11+

- Add PORT=5000 in environment variables (if needed)

# 🧠 Model & Data
- models/recipe_recommendation_model.pkl: Pickled model (vocabulary or vectorizer)

- data/processed/recipes_processed.csv: Preprocessed recipe data with:

   - Title

   - Core_Ingredients

   - Ingredient_Vector

   - Image Link

# ❤️ Acknowledgements
## Thanks to all open-source contributors and dataset providers who made this project possible.
