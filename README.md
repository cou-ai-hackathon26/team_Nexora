# DENGU HUNTER
### AI-Powered Breeding Site Detection, Risk Prediction & Verified Mosquito Prevention

**Team:** Nexora  
**Hackathon:** COU AI Hackathon 2026

## Project Overview

DENGU HUNTER is an AI-powered community surveillance platform designed to identify potential mosquito breeding-site objects, prioritize inspection locations, and track cleanup activities through human review and field response.

Our system combines computer vision, citizen reporting, GPS mapping, risk prioritization, and coordinated field operations.

## Key Features

### 1. AI-Powered Detection
- YOLO-based object detection.
- Identifies potential breeding-site objects such as tires, bottles, vases, coconut exocarp, and drain inlets.
- Detection confidence and inspection recommendations.

### 2. Citizen Reporting
- Photo-based reporting.
- Voice-based reporting.
- Optional GPS coordinates.
- Rain context and previous report information.

### 3. Offline-First Reporting
- Stores reports locally using IndexedDB when internet is unavailable.
- Automatically synchronizes queued reports when connectivity returns.
- Supports photo and voice evidence.

### 4. Risk Prioritization
- Considers detected objects and inspection context.
- Distinguishes uninspected sites from cleanup-reviewed sites.
- Includes logic for zero risk after verified cleanup.

### 5. Admin and Field Worker Workflow
- Human review and approval.
- Worker task assignment.
- Before-and-after photo evidence.
- Final evidence review and reinspection workflow.

### 6. GPS Surveillance
- Location-aware incident reporting.
- Map-based inspection monitoring.

## Technology Stack

- Python
- YOLO / Ultralytics
- OpenCV
- FastAPI
- HTML, CSS, JavaScript
- MySQL
- IndexedDB
- GPS / Mapping

## System Workflow

Citizen Report → Photo & Voice Collection → AI Object Detection → Risk Prioritization → Admin Review → Worker Assignment → Cleanup Evidence → Final Human Review

## Challenge Implementation

**Challenge 1: Voice and Photo Citizen Reporting Without Reliable Internet**

Implemented photo and voice reporting, browser-based offline storage, and automatic synchronization when connectivity returns.

**Challenge 2: Risk Prioritization for Cleared and Uninspected Sites**

Implemented inspection-status-aware risk logic and a zero-score condition for verified cleanup. Full end-to-end field-verification testing remains a limitation.

## Important Limitation

YOLO identifies potential water-holding objects. It does not directly detect dengue infection or mosquito species. Final cleanup decisions require human review and appropriate field verification.

## Team

**Nexora — COU AI Hackathon 2026**
