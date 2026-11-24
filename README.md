# DengueSpot - No More Dengue

An AI-powered system that detects dengue mosquito breeding sites from smartphone photos, assesses risk using weather and location, and gives practical advice in Sinhala and English.

## How it works
1. User takes a photo of their surroundings
2. A YOLO model detects breeding sites (tyres, containers, coconut shells, stagnant water)
3. Uncertain detections are verified by a vision LLM
4. An AI agent checks recent rainfall and official dengue guidelines (RAG)
5. The user gets a risk level and clear advice; reports appear on a hotspot map

## Tech stack
- **Detection:** Ultralytics YOLO, OpenCV, Roboflow, Google Colab
- **Agent:** LLM API with tool calling, Open-Meteo weather API, RAG
- **App:** React + Tailwind (frontend), Flask/FastAPI (backend), SQLite

## Project structure
| Folder | Contents |
|---|---|
| backend/ | API server and AI agent |
| frontend/ | React web app |
| notebooks/ | Model training notebooks |
| models/ | Trained models (not uploaded) |
| data/ | Dataset info (images stored separately) |
| docs/ | Report, diagrams and research notes |

## Status
In development - AI Project module
