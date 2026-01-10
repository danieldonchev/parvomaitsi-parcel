# 3D Viewer Application

## Project Overview
This is a 3D architectural model viewer application that displays property models using GLB 3D files. The application allows users to view architectural models with or without roofs and includes functionality for adding notes.

## Files
- `viewer.html` - Main HTML file containing the complete 3D viewer application
- `parcel-with-roof.glb` - 3D model file with roof (361.396 KB)
- `parcel-no-roof.glb` - 3D model file without roof (361.396 KB)
- `parcel.glb` - Main 3D model file (3.2 MB)

## Features
- Interactive 3D model viewing using Google's model-viewer component
- Toggle between models with and without roof
- Responsive design that works on mobile devices
- Legend showing room type colors
- Notes section for user comments
- Camera controls for rotation, zoom, and panning
- Toast notifications for user feedback
- Fullscreen mode for both desktop and mobile viewing

## Technical Details
- Built with HTML, CSS, and JavaScript
- Uses `model-viewer` web component from Google for 3D rendering
- Responsive design with mobile-friendly controls
- Interactive UI with toggle buttons
- Basic note-taking functionality (API endpoints are placeholders)
- Uses CSS for styling and layout
- Implements camera controls for 3D navigation
- Fullscreen functionality with custom CSS and JavaScript

## Usage
1. Open `viewer.html` in a modern web browser
2. Use the toggle buttons to switch between models with and without roof
3. Interact with the 3D model using mouse controls:
   - Left-click + drag to rotate
   - Scroll to zoom in/out
   - Right-click + drag to pan
4. Use the "Покажи/Скрий" button on mobile to show/hide legend and notes
5. Add notes using the text area and submit button

## Notes
- The note functionality requires a backend API endpoint to be configured (currently uses placeholders)
- All GLB files are excluded from this documentation as requested
- The application is designed to be self-contained in a single HTML file

## Development
This project demonstrates a complete 3D viewer implementation using web technologies. It includes both the frontend interface and the logic for switching between different 3D models.

## Dependencies
- Google's model-viewer web component (loaded via CDN)
- Modern web browser with support for WebGL and ES6 JavaScript