---
title: "Visión Computacional para seguimiento posicional de jugadores y cuantificación de saltos en voleybol"
collection: advising
category: advisor
type: "Undergraduate Thesis (Memoria de Título)"
permalink: /advising/2026-03-01-benjamin-araya
venue: "Universidad Diego Portales, Escuela de Informática y Telecomunicaciones"
date: 2026-03-01
location: "Santiago de Chile"
student: "Benjamín Araya"
status: "In progress"
---

**Student:** Benjamín Araya  
**Degree:** Undergraduate Thesis (Memoria de Título)  
**My Role:** Primary Advisor (Profesor Guía)  
**Institution:** Universidad Diego Portales, Escuela de Informática y Telecomunicaciones  
**Location:** Santiago de Chile  
**Status:** In progress


### Overview

This thesis develops a computer vision system for positional tracking of volleyball players from conventional video footage. The pipeline integrates person detection with YOLO models, multi-object tracking via ByteTrack, automatic court calibration, planar homography, volleyball-specific spatio-temporal rules, and identity consolidation to transform raw detections into auditable top-down trajectories. On top of these trajectories, the system generates heatmaps, tactical visualizations, and jump-related metrics. The work targets coaches and technical staff who lack access to expensive commercial tracking systems, dedicated cameras, or wearable sensors — offering a functional, extensible baseline for spatial-occupancy analysis and jump quantification.

### Key Technologies

- Object detection: YOLOv8, YOLO11, and YOLO12 (comparative evaluation)
- Multi-object tracking with ByteTrack
- Automatic court calibration via temporal median, HSV/Lab masks, and geometric hypothesis validation
- Planar homography for top-down (bird's-eye) projection
- **RedLock**: custom heuristic layer for identity stabilization, side-of-court consistency, and identity inheritance
- Temporal post-processing for jump-event quantification from trajectory data

### Impact

Provides an auditable, low-cost alternative to commercial player-tracking systems for volleyball technical staff. On 99 manually annotated positions, the system achieved **87.88% strict zonal accuracy** and **96.97% accuracy with zone adjacency**, supporting its use for spatial-occupancy analysis. For aggregate jump counting per clip, the system reached **F1 = 0.846** (precision 0.841, recall 0.851) over 87 manually observed jumps, showing consistent estimation of overall jump load — a key metric for load management and injury prevention in players who repeatedly execute net actions.
