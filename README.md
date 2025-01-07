Building a weather data collection system using AWS S3 and OpenWeather API

# Real-Time Weather Data Hub

## Project Overview
This project is a Weather Data Collection System demonstrating DevOps principles such as:

- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code (Iac)
- Version Control (Git)
- Python Development
- Error Handling/Debugging

## Key Features
- Fetches real-time weather data for multiple cities using OpenWeather API
- Displays temperature (°F), humidity, and weather conditions
- Securely saves weather data in AWS S3 using timestamps for unique identification and historical tracking
- Dyanamically supports multiple cities with tracking data

## Technical Architecture
- **Language:** Python 3.x
- **Cloud Provider:** AWS (S3)
- **External API:** OpenWeather API
- **Dependencies:** 
  - boto3 (AWS SDK)
  - python-dotenv
  - requests

```markdown
## Project Structure
weather-dashboard/
  src/
    __init__.py
    weather_dashboard.py
  tests/
  data/
  .env
  .gitignore
  requirements.txt

## Setup Instructions
OpenWeather API Key: Create a free account at OpenWeather to get your API key.

Utilized VScode for efficiency

1. Install dependencies:
pip install -r requirements.txt

2. Configure environment variables (.env):
OPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name

3.Configure AWS credentials:  ## Must have AWS Key and Secret Key
aws configure 

5. Run the application:
python3 src/weather_dashboard.py


What I Learned:

This project demonstrates how to integrate multiple technologies to create a robust and scalable Weather Data Collection System. By leveraging APIs, cloud storage, and Python’s simplicity, you can efficiently collect and store data for further analysis or display.

Future Enhancements:
Alerts for extreme weather conditions
Implement data visualization
Create automated testing
Set up CI/CD pipeline
