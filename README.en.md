# 🎓🍅♨️ Study Time Tracker & Pomodoro Timer

> [简体中文](README.md) | ENGLISH

A simple and efficient single HTML Pomodoro timer application that helps users track study time and manage time effectively.

## 📋 Project Overview

This project uses a single HTML file architecture without any external framework dependencies, implemented with native HTML, CSS, and JavaScript. The application includes three core features:

- 🎓 **Total Study Time Tracker**: Accurately records and accumulates user's effective study time
- 🍅 **Pomodoro Timer**: Customizable countdown focus tool with an intuitive circular progress bar
- ♨️ **Idle Timer**: Independent break countdown tool with a linear progress bar

## ✨ Key Features

### 🎓 Study Time Tracker

- Precise time tracking to the second
- Persistent data storage (using `localStorage`)
- Clear display in "hours:minutes" format
- Data is preserved even after closing the page

### 🍅 Pomodoro Timer

- Customizable countdown duration (default 25 minutes)
- Intuitive circular progress bar display
- Complete control functions: start, pause, stop
- Automatically adds elapsed time to total study time when countdown ends or is stopped
- Supports browser notifications and sound alerts

### ♨️ Idle Timer

- Customizable countdown duration (default 5 minutes)
- Clean linear progress bar display
- Independent timing function that doesn't affect study time statistics
- Also supports start, pause, and stop controls

### 📱 Responsive Design

The application uses responsive layout that automatically adapts to different screen sizes:

- **Large screen devices** (> 1200px): 2x2 grid layout
- **Medium screen devices** (768px - 1200px): Horizontal three-column layout
- **Small screen devices** (< 768px): Vertical compact layout

## 🚀 How to Use

1. Simply open the [`index.html`](index.html) file in your browser to start using it
2. No need to install any dependencies or server environment
3. All data is automatically saved in browser local storage

### Basic Operations

1. **Set Time**: Click on the time input field to customize the duration of the Pomodoro or Idle timer
2. **Start Timer**: Click the ▶️ button to start the countdown
3. **Pause/Resume**: Click the ⏸️ button to pause or resume the timer
4. **Stop Timer**: Click the ⏹️ button to stop the timer (Pomodoro timer will add elapsed time to total study time)

## 🛠️ Technical Implementation

### Tech Stack

- **Frontend**: Native HTML, CSS, JavaScript
- **Data Storage**: Browser `localStorage`
- **Styling**: Native CSS, no external dependencies, with support for dark and light themes

### Core Architecture

- **Data Management Module**: Unified management of time data storage and formatting
- **Pomodoro Timer Controller**: `PomodoroTimer` class, handles all Pomodoro timer logic
- **Idle Timer Controller**: `IdleTimer` class, handles all idle timer logic
- **Responsive Layout**: Uses CSS Grid and Flexbox to achieve adaptive layout

### Data Structure

```json
{
  "totalStudyTime": 0,
  "pomodoroTime": 1500,
  "idleTime": 300
}
```

## 📄 License

This project is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International](LICENSE) license.

## 📖 Design Documentation

For detailed design documentation, please refer to [`docs/design.md`](docs/design.md).

## 🤝 Contributing

Issues and Pull Requests are welcome to improve this project!

## 📝 Changelog

### Initial Version

- Implemented basic Pomodoro and Idle timer functionality
- Added study time tracking feature
- Implemented responsive layout
- Added persistent data storage
- Support for browser notifications and sound alerts
