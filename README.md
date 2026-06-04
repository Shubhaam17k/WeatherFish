# WeatherFish 🐟🌤️

An AI-powered personal weather intelligence app that combines real-time weather data
with smart AI suggestions, Google Calendar integration, and a conversational weather assistant.

## Features
- 🔐 Google Sign-in (OAuth2)
- 🌦️ Real-time weather search by city or postal code
- 🤖 AI-generated personalized weather reports
- 💬 Chat with AI weather assistant (Llama 3.1)
- 📅 Google Calendar integration for event-based weather alerts
- 📍 Save your favourite places (work, gym, shopping etc.)
- 👕 Smart suggestions — umbrella, clothing, activity tips
- 🔊 Multiple AI voice personas
- 🌍 Multilingual support

## Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | FastAPI (Python) |
| Database | MongoDB |
| AI Chat | Llama 3.1 via Ollama |
| AI Reports | Flan-T5 (HuggingFace) |
| Weather Data | Open-Meteo (free) |
| Auth | Google OAuth2 |
| Frontend | React |

## Project Structure

```
WeatherFish/
├── Backend/         # FastAPI backend
│   ├── app/
│   │   ├── models/
│   │   ├── routers/
│   │   └── services/
│   ├── .env
│   └── requirements.txt
└── Frontend/        # React frontend
```

## Getting Started

### Backend
```bash
cd Backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python -m app.main
```

### Frontend
```bash
cd Frontend
npm install
npm start
```

## Environment Variables
Create a `.env` file in `Backend/` folder:
```
GOOGLE_CLIENT_ID=your_client_id
GOOGLE_CLIENT_SECRET=your_client_secret
MONGODB_URL=mongodb://localhost:27017
MONGODB_DB=weatherfish
SECRET_KEY=your_secret_key
```

## Author
Shubhamkumar Vijaykumar Kushwaha
