# DENGUE HUNTER

### AI-Powered Breeding Site Detection, Risk Prediction & Verified Mosquito Prevention

**Team Nexora | COU AI Hackathon 2026**

## 1. Project Overview

DENGUE HUNTER is an AI-powered mosquito breeding site identification and management system designed to support proactive dengue prevention.

The system uses computer vision to identify potential mosquito breeding objects from images, calculate inspection priorities, and coordinate cleanup activities through a structured citizen, reviewer, and worker workflow.

Rather than detecting mosquitoes directly, DENGUE HUNTER focuses on identifying potential breeding environments before they become a greater public health risk.

## 2. Problem Statement

Traditional dengue prevention depends heavily on manual inspection and reactive intervention.

Major challenges include:

- Delayed identification of potential breeding sites.
- Inefficient inspection and cleanup prioritization.
- Limited internet connectivity in some areas.
- Lack of structured cleanup evidence and follow-up.
- Difficulty coordinating citizens and field workers.

## 3. Proposed Solution

DENGUE HUNTER combines AI-based object detection, rule-based risk assessment, location tracking, offline reporting, and human-reviewed cleanup evidence.

**Detect → Prioritize → Locate → Respond → Verify**

## 4. Key Features

- AI-powered mosquito breeding object detection.
- YOLO-based image analysis.
- Rule-based inspection priority scoring.
- Citizen image and voice reporting.
- Offline report storage and synchronization.
- GPS-based location tracking.
- Citizen, Reviewer, and Worker workflows.
- Inspection and cleanup task management.
- Before-and-after cleanup evidence.
- Human review and reinspection decisions.
- Drone mission simulation.
- Risk monitoring dashboard.

## 5. AI Model

The system uses a trained YOLO object detection model to identify potential mosquito breeding objects.

Example detection categories:

- Tire
- Bottle
- Vase
- Coconut Exocarp
- Drain Inlet

**Model file:** `models/f2_best.pt`

The model identifies potential breeding objects rather than directly detecting mosquitoes, larvae, or dengue infection.

## 6. System Architecture

Citizen Image and Voice Report
→ FastAPI Backend
→ YOLO Object Detection
→ Risk Assessment
→ Reviewer Decision
→ Worker Assignment
→ Cleanup Evidence
→ Final Review

## 7. Technology Stack

| Component | Technology |
|---|---|
| Artificial Intelligence | YOLO, Ultralytics |
| Backend | Python, FastAPI |
| Image Processing | OpenCV |
| Frontend | HTML, CSS, JavaScript |
| Offline Storage | IndexedDB |
| Communication | REST API |
| Model | f2_best.pt |
| Version Control | GitHub |

## 8. Repository Structure

| File / Directory | Description |
|---|---|
| `app/` | Backend application |
| `app/__init__.py` | Python package initialization |
| `app/engine.py` | Core detection and processing logic |
| `app/main.py` | FastAPI application |
| `models/f2_best.pt` | Trained YOLO model |
| `data/drone_simulations/` | Drone simulation data |
| `index.html` | Main frontend interface |
| `roles.html` | Role-based interface |
| `app.js` | Frontend application logic |
| `styles.css` | Frontend styling |
| `requirements.txt` | Python dependencies |
| `setup_local.py` | Local setup script |
| `.env.example` | Environment configuration example |
| `.gitignore` | Git exclusion rules |
| `BACKEND_README.md` | Backend documentation |
| `project.docx` | Project documentation |
| `LICENSE` | Repository license |

## 9. Installation and Setup

### Clone the Repository

`git clone https://github.com/cou-ai-hackathon26/team_Nexora.git`

`cd team_Nexora`

### Create a Virtual Environment

`python -m venv .venv`

### Activate the Environment (Windows CMD)

`.venv\Scripts\activate`

### Install Dependencies

`pip install -r requirements.txt`

### Start the Backend

`python -m uvicorn app.main:app --reload`

### Backend API

http://127.0.0.1:8000

### API Documentation

http://127.0.0.1:8000/docs

### Start the Frontend

Open another terminal from the repository directory and run:

`python -m http.server 5500`

Open the following address in a browser:

http://127.0.0.1:5500

Ensure the frontend API configuration matches the backend address. Refer to the backend documentation for additional environment configuration.

## 10. Innovation
