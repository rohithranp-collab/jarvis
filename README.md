# jarvis
# Jarvis

Jarvis is an AI agent application with a web interface. The backend is built with FastAPI and the frontend is plain HTML, CSS and JavaScript.

## Features

- Web chat interface served from the `static` folder
- FastAPI backend with async endpoints
- System information support via `psutil`
- Configuration through a `.env` file

## Project Structure

```
jarvis/
├── app.py          # FastAPI backend
├── run.py          # Launcher script
├── README.md
└── static/
    ├── index.html  # Frontend page
    ├── style.css   # Styles
    └── app.js      # Frontend logic
```

## Requirements

- Python 3.10 or newer
- Packages: `fastapi`, `uvicorn`, `pydantic`, `python-dotenv`, `psutil`

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/rohithranp-collab/jarvis.git
   cd jarvis
   ```

2. Install dependencies:
   ```
   py -m pip install fastapi uvicorn pydantic python-dotenv psutil
   ```

3. Create a `.env` file in the project folder and add your settings, for example:
   ```
   API_KEY=your_key_here
   ```

## Running

```
py app.py
```

Then open http://127.0.0.1:8080 in your browser.

Run it from inside the `jarvis` folder so the `static` folder is found.

## Troubleshooting

- **Directory 'static' does not exist:** make sure `index.html`, `style.css` and `app.js` are inside a `static` folder next to `app.py`.
- **WinError 10013:** the port is blocked or in use. Change the `port=` value in `app.py`.

## License

this project is under the mit license
