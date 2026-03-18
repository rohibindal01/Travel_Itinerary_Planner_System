# ✈️ AI Travel Itinerary Planner

An AI-powered web application built using **Streamlit** that helps users generate personalized travel itineraries based on their selected city and interests.

---

## 📌 1. Basic Flow of the Project

1. The application starts from `app.py`.
2. Environment variables are loaded using `.env`.
3. Streamlit initializes the web interface.
4. User provides input via a form:
   - City name
   - Interests (comma-separated)
5. On clicking **"Generate Itinerary"**:
   - A `TravelPlanner` object is created.
   - City and interests are passed to the planner.
6. The planner processes the inputs and generates a travel itinerary.
7. The itinerary is displayed on the UI.
8. If inputs are missing, a warning message is shown.

---

## 🛠️ 2. Technologies Used

### 🔹 Frontend
- Streamlit – Interactive web UI

### 🔹 Backend Logic
- Python – Core programming language
- Custom Module:
  - `TravelPlanner` – Handles itinerary generation logic

### 🔹 Utilities
- python-dotenv – Environment variable management

---

## 🏗️ 3. Flow Architecture

        ┌────────────────────┐
        │       app.py       │
        │ (Streamlit App)    │
        └─────────┬──────────┘
                  │
                  ▼
    ┌────────────────────────────┐
    │ User Input Form            │
    │ City + Interests           │
    └─────────┬──────────────────┘
              │
              ▼
    ┌────────────────────────────┐
    │ TravelPlanner              │
    │ (Initialize Object)        │
    └─────────┬──────────────────┘
              │
              ▼
    ┌────────────────────────────┐
    │ Set City & Interests       │
    └─────────┬──────────────────┘
              │
              ▼
    ┌────────────────────────────┐
    │ Generate Itinerary         │
    │ (create_itinerary())       │
    └─────────┬──────────────────┘
              │
              ▼
    ┌────────────────────────────┐
    │ Display Itinerary          │
    │ (Streamlit UI)             │
    └────────────────────────────┘

---

## 📖 4. Information About the Project

The **AI Travel Itinerary Planner** is designed to simplify travel planning by generating customized day-trip itineraries based on user preferences.

### ✨ Key Features

- ✅ Personalized itinerary generation  
- ✅ User-friendly input form  
- ✅ Dynamic content generation  
- ✅ Clean and interactive UI using Streamlit  
- ✅ Modular architecture for scalability  

### ⚙️ How It Works

- The user inputs a **city** and their **interests**.
- The `TravelPlanner` processes this data and generates a structured itinerary.
- The output is displayed instantly in a readable format using Streamlit.

### 🎯 Use Cases

- Quick day-trip planning  
- Personalized travel recommendations  
- AI-based itinerary generation demos  

---

## ▶️ How to Run the Project

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
