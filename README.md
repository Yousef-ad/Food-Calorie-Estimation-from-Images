# Food Calorie Estimation from Images

## Overview

This project estimates the calorie content of food items from images using AI-powered food detection combined with nutritional data from the USDA database. Users upload a photo of their meal, input the serving size, and receive an estimated calorie count for each detected food item.

## Key Features

- **AI-Based Food Detection:** Uses a YOLOv8 model for food recognition.
- **Calorie Estimation:** Integrates USDA API to fetch calories per 100 grams for detected foods and calculates total calories based on serving size.
- **Simple Web Interface:** FastAPI backend serving an easy-to-use upload form.
- **Offline and Online Components:** Food detection runs locally; nutritional data is fetched online.

## Tech Stack

| Tool/Language | Role |
|---------------|------|
| Python        | Backend logic, API handling |
| FastAPI       | Web framework for API and web UI |
| YOLOv8        | Deep learning model for food detection |
| USDA API      | Nutritional data source |

## Development Environment

- OS: Windows 10 (21H2)

## How It Works

- User uploads an image and inputs serving size (in grams).
- YOLOv8 detects food items in the image.
- For each detected food, USDA API is queried to retrieve calories per 100g.
- Estimated calories are calculated based on serving size.
