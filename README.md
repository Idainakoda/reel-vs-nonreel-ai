# reel-vs-nonreel-ai-model
Real-time AI model to classify network traffic as video (reel) or non-video using RandomForest and network flow monitoring.


This project provides an AI-powered system to classify network traffic from social networking platforms (e.g., Facebook, YouTube) into Reel (video-based) and Non-reel (regular browsing/chat) traffic in real-time. It enables user equipment (UE) to dynamically optimize performance based on traffic type and network conditions.

Features

Real-time Detection: Classifies incoming traffic as Reel or Non-reel instantly.

AI/ML Integration: Uses a trained model for accurate predictions.

Dynamic Optimization: Sends adaptive signals to improve user experience under varying network congestion.

Modular Design: Includes separate modules for network monitoring, model management, and app integration.

REST API Ready: Easily integrates with web-based dashboards, analytics, or mobile applications.

Project Structure
├── app.py                # Main backend application integrating AI model and API
├── network_monitor.py    # Monitors real-time network traffic and extracts relevant data
├── model_manager.py      # Manages loading, saving, and updating of the trained model
├── requirements.txt      # Dependencies for the project
├── README.md             # Project documentation


Installation

Clone the repository:

git clone https://github.com/Idainakoda/reel-vs-nonreel-ai


Install dependencies:

pip install - requirements.txt



Usage

Start the application:

python app.py


Send network traffic data to the API endpoint:

Endpoint: /predict

Method: POST

Data format: JSON containing packet information.

View real-time predictions via the dashboard or logs.

Modules
1. app.py

Integrates the trained AI/ML model with a web interface or API.

Handles requests and returns classification results in real-time.

Bridges between AI inference engine and user-facing components.

2. network_monitor.py

Captures live network traffic.

Extracts features required for classification.

Streams data to the prediction service for analysis.

3. model_manager.py

Loads, saves, and updates the trained model.

Handles retraining and model versioning.

Ensures consistent model performance over time.

Commit Message Used

Initial Commit: Added app.py, network_monitor.py, and model_manager.py with detailed descriptions and initial implementation.

Future Improvements

Implement advanced anomaly detection for fake or malicious reel traffic.

Add visualization dashboard with real-time analytics.

Extend compatibility to more SNS platforms.
