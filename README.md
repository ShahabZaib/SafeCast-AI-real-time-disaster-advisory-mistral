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
/real-time-disaster-advisory-mistral/
├── llm_loader.ipynb # Loads Mistral 7B GGUF model
├── live_data_loader.ipynb # Fetches live weather data
├── format_prompt_from_live_data.ipynb # Creates prompt from structured data
├── main.ipynb # Runs full pipeline and outputs advisory
├── .gitignore
├── LICENSE (MIT)


---

## ⚠️ Model Not Included

The `.gguf` model is not hosted in this repository due to size and license restrictions.  
📥 Download from: [Mistral 7B Instruct (GGUF)](https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.2-GGUF)

Place the file in a directory named `Model/` and update your `model_path` accordingly.

---

## 🔐 API Key Required

You'll need a free API key from [OpenWeatherMap](https://openweathermap.org/api).  
Replace the `API_KEY` placeholder in `live_data_loader.ipynb`.

---

## 📋 Requirements

Install all required packages:
Download requirements.txt

```bash
pip install -r requirements.txt

---

## Example Output

📍 Location: Karachi (24.75°N, 67.02°E)
🌡 Temperature: 39°C
🌬 Wind Speed: 12.5 km/h

✅ Final Advisory:
- High temperature detected. Stay hydrated and avoid outdoor activities.
- Risk of dehydration. Keep emergency supplies ready.

---

## 📝 License

MIT License – free to use, modify, and share with credit.
