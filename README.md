# 🌤️ Weather API - Django

A simple RESTful Weather API built using Django and Django REST Framework. This API allows users to fetch real-time weather data for a given city by integrating with a third-party weather service (e.g., OpenWeatherMap).

---

## 🚀 Features

- Get current weather by city name
- RESTful endpoints with JSON responses
- Error handling for invalid requests
- Configurable API key integration
- Clean, modular Django project structure

---

## 🛠️ Tech Stack

- Python 3.x  
- Django 4.x  
- Django REST Framework  
- Requests (for external API calls)

---

## 📦 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/weather-api-django.git
   cd weather-api-django
   Create a virtual environment

2. **Create a virtual environment**
   ```bash
    python -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    Install dependencies

3. **Install dependencies**
   ```bash
    pip install -r requirements.txt
    Set up environment variables
    Create a .env file in the root directory and add:

4. **Set up environment variables 'Create a .env file in the root directory and add:'**
   ```bash
    WEATHER_API_KEY=your_openweathermap_api_key
    

5. **Run the server**
   ```bash
    python manage.py runserver
    
## 📡 API Endpoint
    GET /api/weather/?city=CityName

## 🔸 Example Request
```
GET /api/weather/?city=London
```
## 🔸 Example Response
```
{
  "city": "London",
  "temperature": "15°C",
  "description": "Partly cloudy",
  "humidity": 72,
  "wind_speed": "5.1 m/s"
}
```

## 📁 Project Structure
```
weather_api/
├── weather/              # App with API logic
│   ├── views.py
│   ├── urls.py
│   └── ...
├── weather_api/          # Project settings
├── manage.py
└── requirements.txt
```
## ✨ Future Improvements
 *> Add 5-day forecast support*
 *> Token-based authentication*
 *>City auto-complete suggestions*

## 📄 License
This project is licensed under the MIT License.

**Made with ❤️ using Django**
