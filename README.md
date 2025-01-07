Building a weather data collection system using AWS S3 and OpenWeather API

# Weather Data Collection System

## Project Overview
This project is a Weather Data Collection System that demonstrates core DevOps principles by combining:
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
<img width="1154" alt="Screenshot 2024-06-26 at 3 04 44 PM" src="https://github.com/user-attachments/assets/7995df22-d163-4f20-957e-af14fdf50110" />

2. Configure environment variables (.env):
OPENWEATHER_API_KEY=your_api_key
AWS_BUCKET_NAME=your_bucket_name

3.Configure AWS credentials:
aws configure

5. Run the application:
python3 src/weather_dashboard.py
<img width="380" alt="Screenshot 2025-01-07 at 5 58 56 PM" src="https://github.com/user-attachments/assets/a44d1768-622d-49c8-8818-d6790429cb00" />
![Screenshot 2025-01-07 at 6 01 08 PM](https://github.com/user-attachments/assets/63f66cc5-7af2-4f68-8cd0-a03f2bc1c3fe)

What I Learned

AWS S3 bucket creation and management
Environment variable management for secure API keys
Python best practices for API integration
Git workflow for project development
Error handling in distributed systems
Cloud resource management

Future Enhancements

Add weather forecasting
Implement data visualization
Add more cities
Create automated testing
Set up CI/CD pipeline
