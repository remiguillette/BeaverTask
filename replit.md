# Beavertask - Task Management Kiosk

## Overview
Beavertask is a beautiful, self-contained task management application built with vanilla HTML, CSS, and JavaScript. It features a dark-themed kiosk interface with orange accent colors, perfect for managing tasks with style.

## Features
- ✅ **Full CRUD Operations**: Create, Read, Update (Edit), and Delete tasks
- ✅ **Task Status Tracking**: Automatic status detection (Pending, Completed, Overdue)
- ✅ **Filtering**: Filter tasks by All, Pending, Completed, or Overdue status
- ✅ **Search**: Search tasks by title, description, or tag
- ✅ **Calendar View**: Interactive calendar showing tasks by due date
- ✅ **QR Code Sharing**: Generate QR codes to share task details
- ✅ **Local Storage**: All tasks are saved in browser localStorage (no backend required)
- ✅ **Responsive Design**: Works on desktop and mobile devices

## Technology Stack
- **Frontend**: Pure vanilla HTML5, CSS3, and JavaScript (no frameworks)
- **Storage**: Browser localStorage for data persistence
- **QR Codes**: QRCode.js library from CDN
- **Server**: Python http.server for development

## Project Structure
```
/
├── index.html          # Complete application (HTML, CSS, JS)
└── replit.md          # Project documentation
```

## How to Use

### Adding a Task
1. Click the "New task" button or select "Add task" from the Tasks menu
2. Fill in the task details:
   - Title (required)
   - Description (optional)
   - Due date (required)
   - Tag (optional)
3. Click "Save task"

### Managing Tasks
- **Edit Task**: Click the "Edit" button to modify an existing task
- **Mark Complete/Pending**: Click the status button on any task card
- **Delete Task**: Click the "Delete" button on any task card
- **Share Task**: Click "Share QR" to generate a QR code for the task
- **Search Tasks**: Use the search box to find tasks by title, description, or tag
- **Filter Tasks**: Use the filter buttons to view specific task types

### Calendar View
1. Click "Calendar" from the Tasks menu
2. Navigate between months using Prev/Next buttons
3. View tasks on their due dates
4. Completed tasks are shown in green, pending tasks in orange

## Task Status Logic
- **Completed**: Task is marked as complete
- **Overdue**: Task is not complete and due date has passed
- **Pending**: Task is not complete and due date is today or in the future

## Data Storage
All tasks are stored in your browser's localStorage under the key `beavertask_tasks`. Data persists between sessions but is specific to each browser/device.

## Design System
- **Background**: Radial gradient from dark purple to black
- **Accent Color**: Orange (#f89422)
- **Card Background**: Semi-transparent dark cards with blur effects
- **Text**: Light gray/white text for readability
- **Status Colors**:
  - Success (Completed): #26d9a6 (green)
  - Pending: #ffb347 (orange)
  - Overdue: #f45c84 (pink/red)

## Recent Changes
- **October 14, 2025**: 
  - Initial implementation with task list, calendar view, and QR code sharing
  - Added full CRUD operations including Edit functionality for updating existing tasks
  - Implemented localStorage persistence for offline-first experience
  - Task status tracking with automatic overdue detection

## User Preferences
- Vanilla HTML/CSS/JavaScript only (no React or frameworks)
- Dark theme with orange accents
- Kiosk-style interface
- Local storage for data persistence
