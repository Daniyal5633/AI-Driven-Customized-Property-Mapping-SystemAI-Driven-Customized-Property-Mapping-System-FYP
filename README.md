# Estate Edge Dashboard

A modern web application for analyzing building properties, including height measurement and blight detection using AI models.

## Features

- Interactive dashboard with Material-UI components
- Building height measurement using computer vision
- Blight detection with TensorFlow.js
- Interactive map for location selection
- Property management system

## Prerequisites

- Node.js (v14 or later)
- Python (v3.8 or later)
- pip (Python package manager)

## Setup

### Frontend Setup

1. Install Node.js dependencies:
```bash
cd dashboard
npm install
```

2. Create a `.env` file in the dashboard directory with:
```
REACT_APP_API_URL=http://localhost:5000
```

### Backend Setup

1. Create a Python virtual environment:
```bash
cd server
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install Python dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application

1. Start the backend server:
```bash
cd server
python app.py
```

2. In a new terminal, start the frontend development server:
```bash
cd dashboard
npm start
```

The application will be available at http://localhost:3000

## Project Structure

```
dashboard/
├── src/
│   ├── components/
│   │   ├── Dashboard.tsx
│   │   ├── GeoLocation.tsx
│   │   ├── HeightAnalysis.tsx
│   │   └── BlightDetection.tsx
│   └── App.tsx
├── server/
│   ├── app.py
│   └── requirements.txt
└── README.md
```

## AI Models

### Height Measurement

The height measurement model uses computer vision techniques to estimate building heights from single images. It integrates with the existing height calculation model in the project.

### Blight Detection

The blight detection model uses a convolutional neural network trained to identify signs of building deterioration. It can:
- Detect multiple areas of concern in a single image
- Provide confidence scores for each detection
- Generate an overall blight score for the building

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 
