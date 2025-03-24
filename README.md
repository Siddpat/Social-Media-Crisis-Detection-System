# Social Media Crisis Detection System 

A comprehensive pipeline for detecting mental health crises in social media posts using NLP, sentiment analysis, and geospatial mapping.


## Project Overview
This system helps identify at-risk individuals by analyzing social media posts through three key phases:
1. **Data Extraction**: Collects mental health-related posts from Reddit
2. **Risk Assessment**: Classifies posts by sentiment and crisis level
3. **Geospatial Analysis**: Maps crisis concentrations and identifies high-risk areas

## 🛠Features
### Task 1: Data Pipeline
- API integration for Reddit using Reddit API
- 15-keyword filter (`depression`, `suicidal`, etc.)
- Advanced text cleaning pipeline including removal of emojis.
- CSV/JSON output with engagement metrics

### Task 2: Risk Classification
- Dual sentiment analysis (VADER + TextBlob)
- 3-tier risk assessment:
  | Risk Level | Criteria | Example |
  |------------|----------|---------|
  | High       | Direct crisis language | "I want to end it all" |
  | Moderate   | Help-seeking behavior | "Struggling with addiction" |
  | Low        | General discussion | "Mental health awareness matters" |

### Task 3: Crisis Mapping
- Hybrid geocoding (metadata + NLP extraction)
- Interactive Folium heatmaps
- Top 5 crisis location identification

