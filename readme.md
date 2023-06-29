# YouTube API Project

This project uses the YouTube API to extract data from YouTube channels, playlists, and videos.

## Overview

The YouTube API project is designed to retrieve channel data, playlist information, and video details from YouTube using the YouTube Data API. It allows users to extract data such as channel name, subscriber count, video count, video statistics, and comments for analysis or further processing. This project aims to provide a convenient way to gather insights from YouTube data programmatically.

## Prerequisites

- Python 3.9 or higher
- `googleapiclient` library
- `pymongo` library
- `mysql-connector-python` library
- `streamlit` library
- YouTube Data API key (Get one from the Google Developers Console)

## Installation

1. Clone the repository:


2. Install the required libraries using pip:


3. Set up the YouTube Data API:

- Go to the Google Developers Console: [https://console.developers.google.com/](https://console.developers.google.com/)
- Create a new project and enable the YouTube Data API for the project.
- Generate an API key and replace the `api_key` variable in the code with your API key.

## Usage

```python
# Import necessary libraries
from googleapiclient.discovery import build
from pymongo import MongoClient
import mysql.connector
import streamlit as st

# Initialize YouTube API
api_key = "YOUR_API_KEY"
youtube = build("youtube", "v3", developerKey=api_key)

# Function to retrieve channel data
def extract_data(channel_ids):
    # Your code here...

# Example usage
channel_ids = ['UC5PstSsGrRwj2o6asQpC4Rg', 'UC-lHJZR3Gqxm24_Vd_AJ5Yw', 'UCq-Fj5jknLsUf-MWSy4_brA','UC295-Dw_tDNtZXFeAPAW6Aw', 'UCRi5VBEe4iFJ9RllWkAU35g',
               'UCpVm7bg6pXKo1Pr6k5kxG9A', 'UCa6vGFO9ty8v5KZJXQxdhaw', 'UC7_YxT-KID8kRbqZo7MyscQ', 'UCBcWMhWcCZZVhwps-SWgag', 'UCX6OQ3DkcsbYNE6H8uQQuVA']



