# Dynatrace App Performance Monitoring Tool

## Overview

This script automates the process of:

1. Logging into Dynatrace through the Microsoft single sign-on (SSO) flow.
2. Scraping performance metrics from specified Dynatrace dashboards.
3. Capturing error rates and response times for web requests.
4. Generating a comprehensive PowerPoint presentation with the collected metrics.

## Features

- **Automated Login**: Handles Microsoft SSO authentication flow
- **Multi-App Support**: Monitors Safaricom App, mPesa Consumer, Business App, and Partner App
- **Platform-Specific Metrics**: Differentiates between Android and iOS metrics where applicable
- **Web Request Analysis**: Tracks error rates for safaricom.co.ke and safaricom.com domains
- **Response Time Monitoring**: Captures and analyzes web request response times
- **Automated Reporting**: Creates professional PowerPoint presentations with dated timeframes

## Installation

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Ensure you have Chrome browser installed (ChromeDriver will be managed by Selenium)

3. Create a `config.json` file with your Microsoft login credentials:
   ```json
   {
     "email": "your.email@safaricom.co.ke",
     "password": "your_password"
   }
   ```

## Usage

Simply run the main script:

```bash
python main.py
```

The script will:
1. Launch Chrome browser (headless mode can be configured)
2. Log in to Dynatrace using Microsoft SSO
3. Navigate through various dashboards to collect metrics
4. Process and organize the collected data
5. Generate a PowerPoint presentation in the `report_folder` directory with the current date range

## Notes

- **PPTX**: The generated pptx is stored in report folder named as `App_Performance_report_{date & month} 00-00 - {date & month} 23-59.pptx`
  - The folder has a reference pptx for you to compare it with your output at first.
- **Time Periods**: By default, the tool analyzes the past 7 days of data from yesterday 23:59 to 7 days ago at 00:00
- **Target URLs**: The URLs monitored are stored in `urls.py`
- Ensure you have a stable internet access as the time may lapse with poor internet hence the scraper may not find some elements
- Average runtime is 12 minutes
