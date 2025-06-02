# 🌪️ Real-Time Disaster Advisory Generator (Mistral)

This project generates real-time weather-based risk advisories using the **Mistral 7B Instruct** model loaded via `llama-cpp-python`. It fetches live weather data, formats it into a domain-specific prompt, and uses the LLM to generate clear, actionable bullet-point advisories.

---

## 📦 Features

- Loads Mistral `.gguf` model using `llama-cpp`
- Fetches live data from OpenWeather API
- Generates structured, one-time RAG-style prompts
- Outputs real-time disaster advisories
- Modular design: data fetch, prompt formatter, LLM loader

---

## 🧠 Technologies Used

- Python 3.10+
- llama-cpp-python
- OpenWeatherMap API
- Mistral 7B GGUF model (linked below)
- Real-time advisory logic via structured prompts

---

## 📂 Project Structure

