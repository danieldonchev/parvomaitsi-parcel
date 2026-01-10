# 3D Viewer Configuration Documentation

## Overview
This document describes the configuration settings for the 3D viewer application.

## Configuration Parameters

### Model Files
The application uses three GLB 3D model files:
- `parcel.glb` - Main 3D model file (3.2 MB)
- `parcel-with-roof.glb` - 3D model file with roof (361.396 KB)
- `parcel-no-roof.glb` - 3D model file without roof (361.396 KB)

### Model Viewer Component
The model-viewer component is configured with the following properties:
- `src`: Path to the GLB file (initially set to 'parcel-with-roof.glb')
- `alt`: Alternative text for accessibility
- `camera-controls`: Enables camera controls for rotation, zoom, and panning
- `auto-rotate`: Automatically rotates the model
- `shadow-intensity`: Controls shadow intensity (set to 1)
- `exposure`: Controls lighting exposure (set to 0.8)
- `camera-orbit`: Initial camera position (45deg 60deg 80m)
- `min-camera-orbit`: Minimum camera distance (20m)
- `max-camera-orbit`: Maximum camera distance (150m)
- `environment-image`: Environment map (set to 'neutral')

### UI Settings
- `toggle-btn`: Toggle buttons for switching between models with and without roof
- `legend-container`: Legend container with room type colors
- `notes-section`: Notes section for user comments
- `mobile-toggle-btn`: Mobile toggle button to show/hide legend and notes
- `fullscreen`: Fullscreen mode with custom CSS styles

### API Configuration
- `API_ENDPOINT`: Base URL for API calls (currently 'http://176.12.8.77:5082')
- `NOTE_ENDPOINT`: Endpoint for sending notes ('/notes')
- `NOTES_GET_ENDPOINT`: Endpoint for retrieving notes ('/notes')

## Notes
- All configuration is hardcoded in the HTML file
- The application is designed to be self-contained in a single HTML file
- Configuration changes require modifying the HTML file directly
- The application is built with HTML, CSS, and JavaScript, using Google's model-viewer web component
- Responsive design with mobile-friendly controls
- The application uses a simple JavaScript implementation for note functionality with basic error handling