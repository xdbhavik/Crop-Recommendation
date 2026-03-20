# 🌾 Crop Recommendation

A machine learning web app that recommends the most suitable crop to grow based on soil and environmental conditions. Built with Python, Flask, and scikit-learn.

---

## ✨ Features

- 🌱 Recommends the best crop based on soil nutrients and climate data
- 📊 Uses a trained ML model served via a clean Flask web interface
- ⚡ Instant recommendations with a single form submission
- 🎨 Responsive HTML/CSS frontend

---

## 🛠️ Tech Stack

| Layer         | Technology                  |
|---------------|-----------------------------|
| Backend       | Python, Flask               |
| ML Model      | scikit-learn (pickled model)|
| Data Handling | NumPy                       |
| Frontend      | HTML, CSS (Jinja2 templates)|

---

## 📁 Project Structure

```
Crop-Recommendation/
├── app.py              # Flask app — routes and recommendation logic
├── main.py             # Entry point
├── model.pkl           # Trained ML model (serialized)
├── requirements.txt    # Python dependencies
├── templates/          # Jinja2 HTML templates
└── static/             # CSS and static assets
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/xdbhavik/Crop-Recommendation
   cd Crop-Recommendation
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the app**

   ```bash
   python app.py
   ```

4. Open your browser and go to `http://127.0.0.1:5000`

---

## 🧠 How It Works

The user fills in a form with the following soil and climate parameters:

| Input        | Description                          |
|--------------|--------------------------------------|
| **N**        | Nitrogen content in soil             |
| **P**        | Phosphorus content in soil           |
| **K**        | Potassium content in soil            |
| **Temperature** | Ambient temperature (°C)          |
| **Humidity** | Relative humidity (%)               |
| **pH**       | Soil pH value                        |
| **Rainfall** | Rainfall (mm)                        |

These values are passed to the trained `model.pkl`, which recommends the most suitable crop to plant under those conditions.

---

## 📦 Dependencies

```
Flask
numpy
scikit-learn
gunicorn
```

Install all with:

```bash
pip install -r requirements.txt
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or file an issue.

---

## 📄 License

This project is open source. Feel free to use and modify it.

---

*Built with ❤️ by [xdbhavik](https://github.com/xdbhavik)*
