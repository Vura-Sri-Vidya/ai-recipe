# 🍽️ SmartDish

> **AI-Powered Recipe Generator from Food Images**

SmartDish is a full-stack AI-powered web application that transforms a photo of food or ingredients into personalized recipes. Using computer vision and large language models, the application detects ingredients from an uploaded image, generates multiple recipe suggestions, and creates a detailed recipe with nutrition information based on the user's dietary preferences.

---

## 📌 Problem Statement

Many people struggle to decide what to cook using the ingredients already available at home. This often leads to food wastage, time-consuming recipe searches, and difficulty maintaining dietary preferences.

SmartDish solves these challenges by generating personalized recipes directly from an uploaded image.

---

## 🎯 Core Objectives

- Detect ingredients from uploaded food images.
- Generate AI-powered personalized recipes.
- Support multiple dietary preferences.
- Provide nutritional information.
- Save and manage recipes for future use.

---

## ✨ Key Features

- 📸 AI-based ingredient detection from images
- 🤖 Personalized recipe generation
- 🥗 Dietary preference filters (Vegan, Keto, Gluten-Free, High-Protein, etc.)
- 📊 Nutrition analysis (Calories, Protein, Carbs, Fat, Fiber)
- 💡 Three recipe suggestions before generating a complete recipe
- 💾 Save, search, filter, and delete recipes
- 📱 Responsive user interface

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Frontend | React.js, Vite, CSS, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB Atlas, Mongoose |
| AI Models | Groq Vision (LLaMA 4 Scout), Groq LLaMA 3.3 70B |
| File Upload | Multer |
| State Management | React Context API |

---

## 🏗️ System Architecture

```text
                User
                  │
                  ▼
          React Frontend
                  │
          Upload Food Image
                  │
                  ▼
        Express.js Backend
                  │
        Convert Image → Base64
                  │
                  ▼
   Groq Vision (LLaMA 4 Scout)
                  │
      Detect Ingredients
                  │
                  ▼
      User Reviews Ingredients
                  │
                  ▼
   Groq LLaMA 3.3 70B
                  │
      Generate Recipes
                  │
                  ▼
        MongoDB Atlas
                  │
                  ▼
      Display & Save Recipe
```

---

## 🔄 Workflow

1. Upload a food or ingredient image.
2. AI detects the ingredients.
3. Review and edit the detected ingredients.
4. Select an optional dietary preference.
5. Generate three recipe suggestions.
6. Choose one recipe.
7. AI generates a complete recipe with nutrition details.
8. Save the recipe to MongoDB for future access.

---

## 📂 Project Structure

```text
client/
├── src/
│   ├── components/
│   ├── context/
│   ├── hooks/
│   ├── pages/
│   ├── services/
│   └── utils/

server/
├── controllers/
├── routes/
├── models/
├── middleware/
├── services/
└── uploads/
```

---

## 📊 AI Workflow

```text
Image Upload
      │
      ▼
Ingredient Detection (Groq Vision)
      │
      ▼
Ingredient Validation
      │
      ▼
Recipe Suggestions
      │
      ▼
Recipe Generation
      │
      ▼
Nutrition Analysis
      │
      ▼
Save to MongoDB
```

---

## 🚀 Future Enhancements

- 👤 User Authentication
- 🌍 Multi-language Support
- 🎙️ Voice-assisted Recipe Generation
- 🛒 Grocery Shopping List
- 📅 Weekly Meal Planner
- ❤️ Favorite Recipes
- 📱 Mobile Application

---

## 📚 Learning Outcomes

- Full-Stack MERN Development
- AI Integration using Groq APIs
- Image Processing
- Prompt Engineering
- REST API Development
- MongoDB Integration
- React Context API
- Responsive UI Design

---
