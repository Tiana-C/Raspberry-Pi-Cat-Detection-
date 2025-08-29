# Raspberry-Pi-Cat-Detection-
## 🐈 Overview- *Project in progress
This project is a homelab exercise to learn Docker, container networking, and database integration on a Raspberry Pi 4. The end goal is to build an AI &amp; Edge Computing system that detects cats via a USB camera, stores detections in a database, and triggers alerts via AWS (S3 + Lambda + Rekognition + SNS).
## Architecture
## Features Implemented 
- Multi-container stack using Docker Compose v2
- Postgres database with persistent storage
- Adminer web interface for easy DB management
- Custom Python worker container:
  - Connects to Postgres
  - Ensures schema
  - Simulates detections (cat ~33%, dog ~67%)
  - Inserts rows into DB every 10s
- Nginx web server serving a static “Hello Docker” page
