# Store Survey Analysis App

A Streamlit application for analyzing store survey results using natural language queries.

## Features

This app provides a simple interface to query store survey data with natural language:

- **View stores not visited** - See which stores still need to be surveyed
- **Check flyer compliance** - Identify stores without required flyers
- **Analyze flyer comments** - Review and summarize comments about missing flyers

## How to Use

1. Enter one of the following queries in the text box:
   - "How many stores have not been visited?"
   - "Which stores didn't have a flyer?"
   - "Summarize the comments about the flyer"

2. View the results with tables and text-based visualizations

## Setup & Installation

### Local Development
```bash
# Create a virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

### Deployment
This app can be deployed on Streamlit Cloud or any other Python hosting service.

## Data Requirements

The app expects a CSV file named `SurveyResultsExtractShort.csv` with the following columns:
- Banner Name
- Site Code
- Site Name
- Status
- Activity Date
- Does the store have a glass cabinet?
- Where you able to find the flyer?
- Provide notes and what was discussed with the store staff if the flyer was not found.
- And other survey-related columns
