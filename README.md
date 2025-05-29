GLOF-S: Early Prediction, Monitor & Alert System
🌍 A smart, real-time, web-based system for early prediction, monitoring, and alerting of Glacial Lake Outburst Floods (GLOFs). It integrates weather data, satellite insights, and machine learning to assess and alert risk in vulnerable regions.

🔧 Features
📡 Real-time weather and lake data analysis

🤖 ML-based GLOF risk prediction engine

📊 Visualization of monitored lakes and event history

🔔 SMS and log-based alert system

🧠 Offline and online operational capability

🗂️ Project Structure
graphql
Copy
Edit
final_ submission/
│
├── app.py                     # Main Flask app
├── glof_alert_system.py       # Core logic for GLOF prediction
├── glof_events.csv            # Recorded GLOF event data
├── lakes.csv                  # Lake monitoring data
├── test_sms.py                # SMS alert test script
├── glof_alerts.log            # Log file for alerts
├── requirement.txt            # Required Python packages
│
├── static/                    # CSS/JS for UI
├── templates/                 # HTML templates
🚀 Installation
bash
Copy
Edit
# Clone the repo and enter the directory
git clone <your-repo-url>
cd final_ submission

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install required packages
pip install -r requirement.txt
▶️ Running the App
bash
Copy
Edit
python app.py
Access the system in your browser at http://127.0.0.1:5000/

🧪 Testing Alert System
Run the following to simulate SMS alerts:

bash
Copy
Edit
python test_sms.py
You may need to configure SMS API credentials (like Twilio) in the script.

📁 Data Files
lakes.csv: List of glacier lakes being monitored.

glof_events.csv: Past events used for training or reference.

glof_alerts.log: Log file storing real-time alerts and predictions.

📌 Dependencies
Flask

Pandas

Requests

(Optional: Twilio for SMS)

See requirement.txt for full list.

📄 License
Licensed under the MIT License. See LICENSE file for details.
