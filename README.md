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
Project Structure

text
shift-tracker/
├── index.html          # Single HTML file containing everything
├── README.md           # This documentation
└── .gitignore         # Git ignore file
The entire application is contained in a single HTML file for simplicity and easy deployment.

Key Classes

ShiftTrackerApp

Main application controller that orchestrates all functionality:

State management
Event handling
UI rendering
Modal management
AppState

Manages application data and persistence:

Shift storage
Projects and tasks
Payment periods
Theme preferences
Cache invalidation
PaymentCalculator

Handles all payment calculations:

Daily pro-rated amounts
Weekly/monthly totals
Payment status checking
Data filtering and aggregation
DateUtils

Date manipulation utilities:

ISO week number calculation
Date formatting
Week range generation
Date validation
SecurityUtils

Security helpers:

Input sanitization
HTML escaping
Data validation
Installation

Download: Clone or download the index.html file
Deploy: Host on any static web server or use locally
Open: Open in any modern web browser
Install as PWA (optional):

iOS: Share → Add to Home Screen
Android: Menu → Install App
No build process, dependencies, or server required!

Usage Guide

Adding Your First Shift

Click the floating + button
Select a date (cannot be in the future)
Choose a project or task
Add optional notes
Click Save Shift
Tracking Payments

Click Payments button in calendar header
Quick Option: Enter amount and click "Mark Current Week Paid"
Custom Period: Set custom date range and amount
Shifts will automatically show as paid
Viewing Analytics

Switch to Summary tab
Use dropdowns to filter by project/task
View weekly, monthly, and yearly statistics
Expand months in year summary for details
Click Show Unpaid Shifts to see pending payments
Managing Data

Click settings gear icon
Add/remove projects and tasks
Change theme (Professional/Dark)
Export backup or CSV
Import previously saved data
Keyboard Shortcuts

Key	Action
←	Previous week
→	Next week
T	Go to today
Enter	Save (in modals)
Esc	Close modal
Data Structure

javascript
Shift = {
  id: Number,
  date: String (YYYY-MM-DD),
  project: String,
  task: String,
  notes: String (optional)
}

PaymentPeriod = {
  id: Number,
  startDate: String (YYYY-MM-DD),
  endDate: String (YYYY-MM-DD),
  amount: Number,
  description: String,
  status: "paid"
}
Browser Support

Chrome (latest)
Firefox (latest)
Safari (latest, including iOS)
Edge (latest)
Samsung Internet (latest)
Limitations

Local Only: Data is stored only in the browser (cleared if browser data is cleared)
1000 Shift Limit: Prevents performance degradation
No Multi-user: Single user, single device
No Cloud Sync: Manual backup/restore only
Future Enhancements

Cloud sync option
Multiple worker profiles
PDF invoice generation
Email reports
Hourly rate calculations
Overtime tracking
Photo attachments for shifts
Geolocation for job sites
Push notifications for payment reminders
License

MIT License - Free for personal and commercial use

Author

Created for construction workers and contractors to simplify shift tracking and payment management.

Version: 1.0 Beta

Last Updated: February 2025
