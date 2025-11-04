# FIFA 2026 World Cup Prediction System

## Overview
An AI-powered prediction system for FIFA 2026 World Cup matches using real historical data, machine learning, and Monte Carlo simulation. Built with Streamlit, XGBoost, and PostgreSQL.

## Current Status
✅ **Fully operational** - The application is running and ready to use

## Project Structure
```
ModelServingArchitecture/
├── app.py                 # Main Streamlit dashboard
├── models.py              # Database schema (SQLAlchemy)
├── data_collection.py     # Web scraping & data fetching
├── preprocessing.py       # Feature engineering
├── model_trainer.py       # XGBoost training
├── monte_carlo.py         # Tournament simulation
└── scheduler.py           # Automated data refresh
```

## Features
- **Real-time Match Predictions**: XGBoost model predicting win/draw/loss outcomes
- **Tournament Simulation**: Monte Carlo simulation for FIFA 2026 tournament
- **Team Analytics**: FIFA rankings visualization and confederation breakdown
- **Data Explorer**: Browse rankings, matches, and processed features
- **PostgreSQL Database**: Persistent data storage with proper schema

## Technology Stack
- **Frontend**: Streamlit (configured for Replit proxy)
- **ML**: XGBoost, scikit-learn, IsolationForest
- **Data**: pandas, numpy, BeautifulSoup, trafilatura
- **Database**: PostgreSQL (via Replit), SQLAlchemy ORM
- **Visualization**: Plotly

## Configuration
- **Port**: 5000 (configured for Replit webview)
- **Host**: 0.0.0.0 (allows all hosts for proxy compatibility)
- **Database**: PostgreSQL via DATABASE_URL environment variable
- **Deployment**: Configured for autoscale deployment

## How to Use
1. **View the App**: The Streamlit interface is already running in the webview
2. **Make Predictions**: Navigate to "Match Predictions" to predict outcomes
3. **Run Simulations**: Use "Tournament Simulator" for Monte Carlo analysis
4. **Explore Data**: Check "Data Explorer" for raw data insights

## Recent Changes (Import Setup)
- ✅ Fixed database enum type handling for PostgreSQL
- ✅ Fixed data collection array length matching
- ✅ Fixed XGBoost multiclass classification configuration
- ✅ Fixed Streamlit configuration for Replit proxy
- ✅ Configured deployment settings
- ✅ Set up PostgreSQL database integration

## Notes
- Live data sources (FIFA.com, Wikipedia) may be blocked; the app uses cached October 2024 data as fallback
- Model training happens on first load and is cached
- Database tables are created automatically on first run
