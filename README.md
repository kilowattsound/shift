Construction Shift Tracker

A progressive web application (PWA) for construction workers and contractors to track work shifts, manage payments, and visualize earnings. Built with vanilla JavaScript and designed for mobile-first usage.


Features

📅 Shift Management

Calendar View: Visual calendar showing shifts with color-coded status (paid/pending)
Week Navigation: Easy navigation between weeks with keyboard shortcuts (← →)
Day Details: Click on any date to view all shifts for that day
Quick Add: Floating action button to quickly add new shifts
Shift CRUD: Create, read, update, and delete shifts with ease
Swipe Gestures: Swipe left to delete, swipe right to edit (mobile-optimized)
💰 Payment Tracking

Payment Periods: Group shifts into payment periods with custom amounts
Status Indicators: Visual indicators for paid vs pending shifts
Quick Week Payment: Mark entire week as paid with a single click
Pro-rated Calculations: Payments are automatically distributed across days in a period
Unpaid Shifts Filter: View all unpaid shifts grouped by week
📊 Analytics & Reporting

Weekly Summary: Shifts count, total paid, daily average
Monthly Summary: Shifts, paid amount, unpaid days, daily averages
Year Summary: Expandable months with detailed statistics
Year-to-Date: Current year earnings overview
Last Month Comparison: Compare with previous month's performance
Interactive Chart: Visual earnings chart with month-by-month breakdown
Filterable Data: Filter analytics by project or task
⚙️ Customization

Projects & Tasks: Manage custom project and task lists
Themes: Professional light theme and dark theme
Custom Tasks: Add on-the-fly custom tasks when needed
Data Export: Export data as JSON backup or CSV for spreadsheet analysis
Import/Restore: Restore from previously exported backups
📱 Mobile Optimized

Touch-friendly interface with appropriate tap targets
Responsive design works on all screen sizes
PWA capable (installable on iOS/Android)
Safe area insets for modern devices (notch support)
Swipe gestures for quick actions
🔒 Data Management

Local Storage: All data stored locally in browser (no server required)
Data Validation: Automatic data validation and cleanup
Cache System: Optimized performance with intelligent caching
Maximum Limit: Prevents excessive data accumulation (1000 shift limit)
Backup/Restore: JSON export/import for data safety
Technology Stack

Pure HTML5/CSS3 - No frameworks, lightweight
Vanilla JavaScript - ES6+ features, modular architecture
Chart.js - Interactive earnings visualization
Font Awesome - Icons and visual elements
Google Fonts - Inter font family
LocalStorage API - Client-side data persistence
