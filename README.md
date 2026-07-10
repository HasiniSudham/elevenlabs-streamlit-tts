🔊 ElevenLabs Streamlit TTS

A simple web app that converts text into natural-sounding speech using the ElevenLabs API, built with Streamlit.

Features


Convert any text into realistic speech
Choose a custom ElevenLabs voice via Voice ID
Play generated audio directly in the browser
Download the output as an MP3 file


Tech Stack


Python
Streamlit — web app interface
ElevenLabs API — text-to-speech generation
python-dotenv — environment variable management


Setup

1. Clone the repository

bashgit clone https://github.com/HasiniSudham/elevenlabs-streamlit-tts.git
cd elevenlabs-streamlit-tts

2. Create and activate a virtual environment

bashpython -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS/Linux

3. Install dependencies

bashpip install -r requirements.txt

4. Add your API key

Create a .env file in the project root:

ELEVENLABS_API_KEY=your_api_key_here

Get your API key from ElevenLabs → Profile → API Keys.

5. Run the app

bashstreamlit run app.py

The app will open at http://localhost:8501.

Usage


Enter the text you want converted to speech
(Optional) Enter a custom Voice ID from ElevenLabs
Click Generate Speech
Listen to the audio or download it as an MP3


Project Structure

elevenlabs-streamlit-tts/
├── app.py              # Main Streamlit app
├── requirements.txt     # Python dependencies
├── output/              # Generated audio files (not tracked in git)
└── .env                 # API key (not tracked in git)

Notes


The .env file is excluded from version control via .gitignore — never commit your API key.
Voice IDs can be found in your ElevenLabs dashboard under Voices.