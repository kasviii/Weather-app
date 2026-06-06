# Nimbus — AI Weather Intelligence

link: https://kasviii.github.io/Weather-app/
A clean, fully-featured weather app in a single HTML file. No build step, no backend, no required API keys to get started.

![HTML](https://img.shields.io/badge/HTML-single%20file-orange) ![License](https://img.shields.io/badge/license-MIT-blue) ![APIs](https://img.shields.io/badge/weather%20API-free-green)

---

## Features

**Real-time weather**
- Current conditions: temperature, feels-like, humidity, pressure, UV index, visibility, cloud cover
- Wind speed, direction, and gusts with an animated compass
- Sunrise, sunset, daylight duration, and moon phase
- 24-hour hourly forecast with precipitation probability
- 7-day daily forecast with temperature range bars

**AI insights** (powered by Groq — free tier)
- Weather summary briefing
- Outfit recommendations for 3 scenarios (casual, smart casual, active)
- Activity suggestions tailored to conditions
- Health & wellness tips (hydration, UV, exercise safety)
- Travel & logistics advice

**UX**
- City search with live autocomplete (OpenStreetMap)
- GPS location detection
- Recent searches saved across sessions
- °C / °F toggle
- Fully responsive — works on mobile

---

## Stack

| Layer | Service |
|---|---|
| Weather data | [Open-Meteo](https://open-meteo.com) |
| Geocoding | [Nominatim / OpenStreetMap](https://nominatim.org) |
| AI insights | [Groq](https://groq.com) |

---

## About the API key

The Groq key is **never stored in the source code**. It lives only in the visitor's browser `localStorage`. This means:

- Each visitor enters their own key (or skips AI features)
- If you want a personal deployment where your key is pre-loaded, use an environment variable via a build step

---

## Project Structure

```
nimbus-weather/
└── weather-app.html    # Everything — HTML, CSS, JS in one file
└── README.md
```

---

## License

MIT — do whatever you want with it.
