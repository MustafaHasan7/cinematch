##Cinematch

by Hasan Mustafa

## Project Overview

CineMatch is a personalized movie recommendation platform that combines semantic search, content-based filtering, and user taste profiling to deliver intelligent movie discovery experiences.

Unlike traditional keyword-based search systems, CineMatch utilizes Natural Language Processing (NLP) embeddings to understand user intent and recommend films based on contextual meaning, thematic similarity, and individual viewing preferences.

The system integrates movie metadata from TMDB and user rating history imported from Letterboxd to generate personalized recommendations and improve content discovery.

---

## Key Features

* Semantic movie search powered by transformer-based text embeddings
* Personalized recommendation engine based on user rating history
* Hybrid ranking pipeline combining:

  * Semantic similarity scoring
  * Lexical keyword matching
  * Mood and intent-based recommendation boosts
* User taste profile generation from historical ratings
* Movie metadata caching for improved performance
* Explainable recommendation results with recommendation reasoning
* Fast and responsive web interface

---

## Technology Stack

### Backend

* FastAPI
* Python
* SQLite
* SQLAlchemy

### Machine Learning & NLP

* Sentence Transformers (all-MiniLM-L6-v2)
* Scikit-learn
* NumPy
* Pandas

### Frontend

* React
* Vite

### External Services

* TMDB API
* Letterboxd Data Import

---

## Project Structure

backend/
├── services/
│   └── nlp.py
├── engine/
│   └── cinematch.py
├── routers/
│   └── movies.py
├── import_letterboxd.py
└── test_taste_model.py

frontend/
├── src/
├── components/
└── pages/

---

## How It Works

1. Movie metadata is collected and cached locally.
2. Movie descriptions, genres, and titles are converted into semantic embeddings.
3. User rating history is analyzed to generate a personalized taste profile.
4. Search queries are processed through a hybrid recommendation pipeline.
5. Results are ranked using semantic relevance, lexical matching, and personalized preference signals.
6. The system returns explainable recommendations with supporting reasoning.

---

## Academic Declaration

This project was independently designed and developed by Hasan Mustafa as part of the requirements for NLP

All source code, architecture, implementation details, and documentation contained in this repository represent original academic work unless otherwise referenced.

Submitted on: 2 June 2026
