# SaferoadAI 🚗

**AI-Assisted Road Accident Detection Using Computer Vision**

SaferoadAI is an accident-detection project that uses YOLOv8 and OpenCV to analyze traffic videos and display detection results through a Flask web dashboard. It also includes an alert-integration concept for communicating accident information to nearby hospitals.

This repository is an adaptation of an existing open-source project, with local demo configuration and documentation improvements.

## Features

- **Accident detection:** Uses a YOLO-based model to analyze traffic footage.
- **Video processing:** Processes video input and displays the results through a web interface.
- **Flask dashboard:** Provides a browser-based interface for testing the application.
- **Frame capture:** Supports saving frames associated with detected events.
- **Demo alert mode:** Allows local testing without sending real external alerts.
- **Extensible design:** Provides a foundation for future improvements to accident monitoring.

## Technologies Used

- Python
- YOLOv8 and Ultralytics
- OpenCV
- Flask
- HTML, CSS and JavaScript

## Requirements

- Python 3.8 or a compatible version supported by the project's dependencies
- pip
- Git
- The dependencies listed in `requirements.txt`

## Installation

Clone this repository:

```bash
git clone https://github.com/rawatsomya/SaferoadAI.git
cd SaferoadAI
```

Create and activate a virtual environment.

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the project dependencies:

```bash
python -m pip install -r requirements.txt
```

## Running the Flask Dashboard

Start the local application:

```bash
python flask_app.py
```

If the configured port is `5001`, open:

http://127.0.0.1:5001

Use the dashboard to select or upload a supported video and test the available detection workflow.

**Note:** The application may require compatible model files and dependencies to be installed correctly.

## Demo Alert Behaviour

The local demo configuration can print alert messages in the terminal when the external alert service is not configured.

Demo alerts are for testing only. They do not contact hospitals or emergency services. Real alert delivery requires appropriate API configuration and testing.

## Project Structure

| File | Purpose |
|---|---|
| `app.py` | Main accident-detection script |
| `flask_app.py` | Flask web dashboard |
| `SendMessage.py` | Alert messaging and demo-mode handling |
| `NearestHospital.py` | Nearest-hospital lookup integration |
| `Image2Url.py` | Image-to-URL helper |
| `currentLocation.py` | Location-related functionality |
| `model_training.ipynb` | Model training notebook |
| `requirements.txt` | Python dependencies |
| `PROJECT_INFO.md` | Project overview, limitations and future scope |
| `best.pt`, `best_model.pt` | YOLO model files |

## Limitations

- Detection results depend on the trained model and input video quality.
- Model predictions should be evaluated before real-world use.
- Hospital notifications are not active in local demo mode.
- This project is a prototype and is not a replacement for verified emergency-response systems.

## Future Scope

- Evaluate model accuracy on varied traffic footage.
- Reduce false-positive detections.
- Improve incident reporting and dashboard visualizations.
- Test integrations with verified mapping and notification services.
- Explore real-time CCTV input in a controlled environment.

## Attribution and License

This project is based on the original open-source repository by https://github.com/rawatsomya/SaferoadAI.git.
## License

This project is distributed under the MIT License. See `LICENSE.md` for details.