# Climate Guardian AI

Climate Guardian AI is a Python-based environmental risk monitoring and analytics application that combines:

- a **FastAPI backend**
- a **Streamlit dashboard**
- **SQLite** for local persistence
- **Open-Meteo** for live weather data
- optional **n8n / Ollama** workflow integration

The project is designed to help users upload CSV datasets, analyze patterns, inspect simulated model outputs, view execution logs, ask AI-style questions, and check weather information for a city.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Requirements](#requirements)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [How to Use](#how-to-use)
- [API Endpoints](#api-endpoints)
- [Data Flow](#data-flow)
- [Environment and Setup Notes](#environment-and-setup-notes)
- [Project Limitations](#project-limitations)
- [Recommended Improvements](#recommended-improvements)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This repository contains a climate and risk analytics application that provides:

- user authentication
- CSV ingestion and pipeline execution
- model comparison simulation
- feature importance visualization
- risk-based filtering and analytics
- weather lookup by city
- AI assistant interaction through webhook-based services

The app appears to be built primarily for interactive analysis and dashboarding rather than production-grade ML training.

---

## Features

### Backend Features
- Sign up and login endpoints
- CSV upload support
- Multi-file ingestion
- In-memory / SQLite-backed execution logging
- Weather lookup using Open-Meteo
- AI question endpoint
- CORS enabled for frontend access

### Streamlit Dashboard Features
- Login and signup UI
- Multiple dashboard views
- Multi-dataset ingestion
- Interactive analytics studio
- Correlation heatmaps
- Scatter plots, histograms, and 3D visualizations
- Execution logs with CSV export
- AI Risk Assistant interface
- Local fallback responses when external AI workflow is unavailable

### Data and Storage
- Local SQLite databases
- Runtime-generated execution history
- Uploaded CSV data handling
- Filtered exports from dashboard views

---

## Project Structure

```text
proj_1/
├── main.py
├── api.py
├── streamlit_app.py
├── agents/
├── datasets/
└── .gitignore
