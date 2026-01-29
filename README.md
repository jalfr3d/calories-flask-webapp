# Calories Web App (Flask)

A simple Flask web application that calculates **daily calorie needs** based on user input and **current temperature**, which is scraped live from **timeanddate.com** using the city and country provided by the user.

---

## 🚀 Features

- 📏 Calorie calculation based on:
  - Height
  - Weight
  - Age
  - Current outdoor temperature
- 🌡️ Live temperature scraping from **timeanddate.com**
- 🌍 User-defined **city** and **country**
- 🧮 Backend logic separated into reusable modules
- 🧪 Built with Flask and WTForms

---

## 🧠 How It Works

1. The user fills out a form with:
   - Weight (kg)
   - Height (cm)
   - Age
   - Country
   - City
2. The app:
   - Scrapes the current temperature for the given location
   - Passes the data to the calorie calculator
3. The calculated daily calorie requirement is displayed on the page

---

## 🗂️ Project Structure
```bash
├── main.py
├── calorie.py
├── temperature.py
├── temperature.yaml
├── templates/
│ ├── index.html
│ └── calories_form_page.html
├── static/
│ ├── main.css
└── requirements.txt
```
## 🔥 Calorie Calculation

The `Calorie` class:
- Takes `weight`, `height`, `age`, and `temperature`
- Calculates daily calorie needs using internal logic (see `calorie.py`)

---

## 🌡️ Temperature Scraping

The `Temperature` class:
- Scrapes live temperature data from **timeanddate.com**
- Requires:
  - `city`
  - `country`

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone https://github.com/jalfr3d/calories-flask-webapp.git
cd calories-flask-webapp
```
### 2. Install dependencies
```bash
pip install -r requirements.txt
```
### 3. Running the App
```bash
python main.py
```

---

📄 License
- This project is licensed under the MIT License.
