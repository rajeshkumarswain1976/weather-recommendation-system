# Weather Alert & Recommendation Agent

A real-time AI agent that fetches live weather data for any city and generates
actionable recommendations using Google Gemini.

---

### What it does

- Accepts any city name as input
- Fetches real-time weather using Open-Meteo API (no API key needed)
- Detects severe conditions — heavy rain, storms, extreme heat
- Generates health tips and safety recommendations using Gemini AI
- Saves the full report to a local file

---

### How it works
User Input (City)
→ Geocoding API → Coordinates
→ Open-Meteo API → Live Weather Data
→ Gemini AI → Analysis + Recommendations
→ Saved Report

---

### Stack

| | |
|---|---|
| **AI** | Google Gemini 1.5 Flash |
| **Weather** | Open-Meteo API · Open-Meteo Geocoding API |
| **Language** | Python |
| **Libraries** | google-generativeai · requests |

---

### Setup

```bash
# Install dependencies
pip install google-generativeai requests

# Add your Gemini API key in the script
GEMINI_API_KEY = "your_api_key_here"

# Run
python weather_recomm.py
```

---

### Example Output
Enter your city name: Mumbai
--- Weather Report & Recommendations ---
Current weather in Mumbai: 31°C, Rain showers, Wind: 18 km/h
⚠️ Alert: Rain showers detected. Carry an umbrella.
💧 Stay hydrated and avoid waterlogged areas.
🚗 Allow extra travel time due to wet roads.

---

> Disclaimer: AI-generated recommendations. Not a substitute for official weather alerts.
