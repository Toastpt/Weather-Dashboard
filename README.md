Building a weather data collection system using AWS S3 and OpenWeather API

# Real-Time Weather Data Hub

## Project Overview
This project is a Weather Data Collection System demonstrating DevOps principles such as:

- External API Integration (OpenWeather API)
- Cloud Storage (AWS S3)
- Infrastructure as Code (Iac)
- Version Control (Git)
- Python Development
- Error Handling
- Environment Management

## Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple cities tracking
- Timestamps all data for historical tracking

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
Utilized VScode for efficiency

1. Install dependencies:
pip install -r requirements.txt

2. Configure environment variables (.env):
OPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name

3.Configure AWS credentials:
aws configure

5. Run the application:
python3 src/weather_dashboard.py


What I Learned

AWS S3 bucket creation and management
Environment variable management for secure API keys
Python best practices for API integration
Git workflow for project development
Error handling in distributed systems
Cloud resource management

Future Enhancements

Implement data visualization
Create automated testing
Set up CI/CD pipeline
