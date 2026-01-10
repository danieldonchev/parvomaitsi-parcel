# 3D Viewer Application

## Overview
This is a 3D architectural model viewer application that displays property models using GLB 3D files. The application allows users to view architectural models with or without roofs and includes functionality for adding notes.

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
### 1. Open the Application
- Open `viewer.html` in a modern web browser

### 2. View 3D Models
- Use the toggle buttons to switch between models with and without roof

### 3. Interact with the Model
- Left-click + drag to rotate
- Scroll to zoom in/out
- Right-click + drag to pan

### 4. Mobile View
- Use the "Покажи/Скрий" button to show/hide legend and notes

### 5. Add Notes
- Enter text in the text area and click "Изпрати бележка"

### 6. Fullscreen Mode
- Click the eye icon in the top right of the legend to enter fullscreen mode

## Development
### Required Dependencies
- Modern web browser with support for WebGL and ES6 JavaScript
- Google's model-viewer web component (loaded via CDN)

### File Structure
- `viewer.html` - Main HTML file containing the complete 3D viewer application
- `parcel-with-roof.glb` - 3D model file with roof
- `parcel-no-roof.glb` - 3D model file without roof
- `parcel.glb` - Main 3D model file
- `docs/` - Documentation directory

### API Endpoints
The application uses the following API endpoints (currently placeholders):
- `POST /notes` - Send a new note
- `GET /notes` - Retrieve all notes

## Notes
- The note functionality requires a backend API endpoint to be configured (currently uses placeholders)
- The application is designed to be self-contained in a single HTML file
- The application uses a simple JavaScript implementation for note functionality with basic error handling

## Documentation
- API Documentation: `docs/api.md`
- Configuration Documentation: `docs/configuration.md`

## License
This project is open source and available under the MIT license.

## Contributing
Contributions are welcome! Please submit pull requests or open issues for bug reports and feature requests.

## Contact
For questions or support, please contact the project maintainer.

## Acknowledgements
- Google's model-viewer component for 3D rendering
- All contributors to this project