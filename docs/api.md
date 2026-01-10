# 3D Viewer API Documentation

## Overview
This document describes the API endpoints used by the 3D viewer application for note functionality. The application uses a simple REST API to send and retrieve notes.

## Endpoints

### POST /notes
Send a new note to the server.

**Request Body**
```json
{
  "note": "string",
  "timestamp": "ISO 8601 timestamp"
}
```

**Example Request**
```bash
curl -X POST http://176.12.8.77:5082/notes \
  -H "Content-Type: application/json" \
  -d '{"note": "This is a test note", "timestamp": "2026-01-10T10:00:00Z"}'
```

**Success Response (200 OK)**
```json
{
  "status": "success",
  "message": "Note sent successfully"
}
```

**Error Response (500 Internal Server Error)**
```json
{
  "status": "error",
  "message": "Failed to save note"
}
```

### GET /notes
Retrieve all notes from the server.

**Request**
```bash
curl -X GET http://176.12.8.77:5082/notes \
  -H "Content-Type: application/json"
```

**Success Response (200 OK)**
```json
[
  {
    "note": "string",
    "timestamp": "ISO 8601 timestamp"
  },
  {
    "note": "string",
    "timestamp": "ISO 8601 timestamp"
  }
]
```

**Error Response (500 Internal Server Error)**
```json
{
  "status": "error",
  "message": "Failed to retrieve notes"
}
```

## Notes
- The API endpoints are placeholders and need to be implemented on the server side
- The application currently uses a hardcoded IP address (176.12.8.77) and port (5082)
- Error handling is implemented in the frontend to display appropriate toast messages
- Notes are displayed in reverse chronological order (newest first)