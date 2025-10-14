# Beavertask - Samsung-Style Calendar

## Overview
Beavertask is a beautiful Samsung-style calendar application built with vanilla HTML, CSS, and JavaScript. It features a modern, minimalist black design with landscape orientation, perfect for managing tasks and events with style.

## Features
- ✅ **Samsung-Style Design**: Modern, minimalist black interface with landscape orientation
- ✅ **Interactive Calendar**: Full month view with date selection and task display
- ✅ **Task List View**: Dedicated view showing all tasks organized by category (Overdue, Upcoming, No Due Date, Completed)
- ✅ **Task Management**: Create, complete, and delete tasks directly from the calendar or task list
- ✅ **Month Navigation**: Navigate between months with prev/next controls
- ✅ **Date Selection**: Click any date to view and manage tasks for that day
- ✅ **Event Indicators**: Visual dots show which dates have tasks
- ✅ **Today Highlight**: Current date highlighted with orange border
- ✅ **Local Storage**: All tasks are saved in browser localStorage (no backend required)
- ✅ **Responsive Design**: Works on desktop, tablet, and mobile devices

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
1. Click on any date in the calendar to select it
2. Type your task in the input field at the bottom of the details panel
3. Press Enter to create the task

### Managing Tasks
- **Select a Date**: Click any date in the calendar to view tasks for that day
- **Complete a Task**: Click the checkbox next to any task to mark it as complete
- **Delete a Task**: Click the × button on any task to delete it
- **Navigate Months**: Use the left/right arrow buttons to move between months
- **Go to Today**: Click the search icon to jump back to today's date
- **View Task Count**: Dates with tasks show a small orange dot indicator

### Calendar View
1. Use Prev (←) and Next (→) buttons to navigate between months
2. Click any date to view and manage tasks for that day
3. The current date is highlighted with an orange border
4. Selected date is shown with an underline and displays its tasks in the right panel
5. Dates with tasks show a small orange dot indicator

### Task List View
1. Click the Task List icon (fourth icon in sidebar) to view all tasks
2. Tasks are automatically organized into categories:
   - **Overdue**: Tasks past their due date
   - **Upcoming**: Tasks with future due dates (sorted by date)
   - **No Due Date**: Tasks without a due date
   - **Completed**: Finished tasks
3. Toggle task completion by clicking the checkbox
4. Delete tasks using the 🗑️ button
5. Click the Calendar icon to return to calendar view

## Task Status Logic
- **Completed**: Task is marked as complete
- **Overdue**: Task is not complete and due date has passed
- **Pending**: Task is not complete and due date is today or in the future

## Data Storage
All tasks are stored in your browser's localStorage under the key `beavertask_tasks`. Data persists between sessions but is specific to each browser/device.

## Design System
- **Background**: Pure black (#000000) with subtle secondary backgrounds
- **Accent Color**: Orange (#f89422)
- **Card Background**: Dark cards (#0a0a0a, #0f0f0f)
- **Text**: White primary (#ffffff), gray secondary (#999999), muted (#666666)
- **Status Colors**:
  - Completed: Checkbox with orange background
  - Current Day: Orange border (#f89422)
  - Selected Date: White underline indicator

## Recent Changes
- **October 14, 2025** (Latest): 
  - **Added Task List View**: New dedicated view to see all tasks organized by category
  - Added Task List icon to sidebar for easy navigation between calendar and task list views
  - Task list automatically categorizes tasks as Overdue, Upcoming, No Due Date, or Completed
  - Tasks in task list are sorted by due date within each category
  - Can manage tasks (complete/delete) directly from task list view
  
- **October 14, 2025**: 
  - Complete redesign to Samsung-style calendar in landscape orientation
  - Added left sidebar with menu and calendar icons
  - Implemented calendar-first layout with date selection as primary interaction
  - Created details panel on right side showing tasks for selected date
  - Added month navigation with prev/next arrow buttons
  - Implemented visual indicators: orange border for today, underline for selected date, dots for dates with tasks
  - Added floating action button for quick event creation
  - Streamlined task creation: type in input field and press Enter
  - Maintained localStorage persistence for all tasks
  - Responsive design adapts to mobile and tablet devices

## User Preferences
- Vanilla HTML/CSS/JavaScript only (no React or frameworks)
- Samsung-style calendar design with landscape orientation
- Dark theme with orange accents
- Calendar-first interface
- Local storage for data persistence
