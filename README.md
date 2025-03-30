# Email Spam Detection System

A comprehensive email spam detection system using machine learning and modern web technologies.

## Project Structure

This repository contains three main components:

- `webapp-frontend/`: React-based web interface
- `webapp-backend/`: Spring Boot REST API
- `ml-model/`: Machine learning model for spam detection

## Setup Instructions

1. Clone the repository with all submodules:
```bash
git clone --recursive https://github.com/yourusername/email-spam-detection.git
```

2. Initialize and update submodules:
```bash
git submodule init
git submodule update
```

3. Follow the setup instructions in each component's README for specific setup steps.

## Development

To update all submodules to their latest versions:
```bash
git submodule update --remote
```

To work on a specific component:
```bash
cd webapp-frontend  # or webapp-backend or ml-model
git checkout main
git pull
```

## Components

### Frontend (webapp-frontend)
- React-based web application
- Features user authentication and email analysis interface

### Backend (webapp-backend)
- Spring Boot REST API
- Handles authentication and ML model integration

### ML Model (ml-model)
- Python-based spam detection model
- Uses machine learning for email classification

## Contributing

Please refer to individual component repositories for specific contribution guidelines.
