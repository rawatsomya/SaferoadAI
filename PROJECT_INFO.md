# SaferoadAI — Project Overview

## About the Project
SaferoadAI is an AI-assisted road accident detection project that uses computer vision to analyze traffic videos and display results through a Flask web dashboard.

## Technologies Used
- Python
- YOLOv8
- OpenCV
- Flask
- HTML, CSS and JavaScript

## Key Features
- Traffic video analysis
- AI-based accident detection
- Web dashboard for viewing results
- Demo-mode alerts for local testing

## Demo Configuration
The application can run locally without configuring the external alert service. In demo mode, alert messages are printed in the terminal instead of being sent to an external service.

## Limitations
Detection accuracy depends on the model and input video. Demo alerts do not contact hospitals or emergency services.

## Future Scope
- Evaluate detection accuracy on diverse traffic footage
- Improve false-positive handling
- Integrate a verified alert service in a controlled test environment
- Add more detailed incident reports

## Attribution
This project is based on an existing open-source project. Please refer to the repository's original README and MIT license for attribution and licensing details.