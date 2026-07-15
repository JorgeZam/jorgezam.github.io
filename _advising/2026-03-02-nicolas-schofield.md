---
title: "Detección de personas mediante visión computacional para la optimización de alertas en videovigilancia"
collection: advising
category: advisor
type: "Undergraduate Thesis (Memoria de Título)"
permalink: /advising/2026-03-02-nicolas-schofield
venue: "Universidad Diego Portales, Escuela de Informática y Telecomunicaciones"
date: 2026-03-02
location: "Santiago de Chile"
student: "Tomás Schofield"
status: "In progress"
---

**Student:** Tomás Schofield  
**Degree:** Undergraduate Thesis (Memoria de Título)  
**My Role:** Primary Advisor (Profesor Guía)  
**Institution:** Universidad Diego Portales, Escuela de Informática y Telecomunicaciones  
**Location:** Santiago de Chile  
**Status:** In progress


### Overview

This project designs and implements a computer vision-based person detection system aimed at optimizing alerts in the CCTV monitoring center of the security company Vigia. It addresses the information overload faced by operators due to the massive growth in the number of surveillance cameras, which causes visual fatigue and severely reduces the ability to detect suspicious events in real time. The proposed solution is a distributed, decoupled architecture that combines an RTSP ingestion module, a Redis Streams message broker, a pool of inference workers, and a spatio-temporal rule engine that filters alerts by temporal persistence and regions of interest.

### Key Technologies

- Computer Vision and Deep Learning (object detection)
- Ensemble of detection models: YOLOv10, Faster R-CNN, and RT-DETR
- Spatial consensus via Intersection over Union (IoU)
- Distributed architecture: RTSP ingestion, Redis Streams message broker, worker pool for inference
- Spatio-temporal rule engine for alert filtering

### Impact

Development of an intelligent surveillance layer that reduces false alarms and lowers the cognitive load on operators managing hundreds of CCTV cameras. By discarding irrelevant activations and prioritizing meaningful events, the system aims to improve incident response times and enable more efficient use of technological security resources in real-world monitoring operations.

