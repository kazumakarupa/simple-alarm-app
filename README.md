# シンプルアラーム 🔔

A minimalist alarm clock application with a clean, modern UI. Set a specific time and get notified with sound and visual effects when the time arrives.

## Features

- ⏰ **Simple Time-Based Alarms** — Set an alarm for a specific time (HH:MM format)
- 🔊 **Audio Notification** — Multi-frequency beeping sound when alarm triggers
- 🎨 **Visual Feedback** — Animated interface changes and color shifts
- 💾 **Persistent Storage** — Alarm settings saved to localStorage
- 📱 **Responsive Design** — Works on desktop and mobile devices
- 🌐 **No Dependencies** — Pure HTML, CSS, and JavaScript

## How to Use

1. Open `index.html` in your web browser
2. Set the desired time using the hour and minute inputs
3. Click "アラーム設定" (Set Alarm) button
4. When the specified time arrives, the app will alert you with sound and visual effects
5. Click "キャンセル" (Cancel) to disable the alarm

### Keyboard Shortcut
Press **Enter** in the time input fields to quickly set the alarm

## Installation

Simply clone the repository and open the HTML file:

```bash
git clone https://github.com/kazumakarupa/simple-alarm-app.git
cd simple-alarm-app
# Open index.html in your browser
```

Or use a local web server:

```bash
python3 -m http.server 8000
# Then navigate to http://localhost:8000
```

## Technical Details

- **Language**: Vanilla JavaScript (No frameworks or build process)
- **Storage**: Browser localStorage for alarm state persistence
- **Audio**: Web Audio API for dynamic sound generation
- **CSS**: Modern Flexbox layout with animations
- **Responsive**: Mobile-friendly design with adaptive breakpoints

## Browser Support

- Chrome/Chromium 50+
- Firefox 45+
- Safari 12+
- Edge 15+

## Project Structure

```
simple-alarm-app/
├── index.html      # Main application file (HTML + CSS + JS)
└── README.md       # Documentation
```

## Features

### Alarm Management
- Set alarm for specific times (24-hour format)
- Visual indication when alarm is active
- Persistent storage across page reloads

### Notifications
- Web Audio API generated beeping sound
- Color-changing background animation
- Blinking status indicator

### User Experience
- Clean, minimal interface
- Clear status messages in Japanese
- One-click alarm cancellation

## Development

The entire application is contained in a single `index.html` file for maximum portability. No build process or external dependencies are required.

### Key Functions

- `loadAlarmState()` — Load alarm setting from localStorage
- `saveAlarmState()` — Persist alarm state
- `setAlarm()` — Create new alarm with validation
- `cancelAlarm()` — Disable current alarm
- `checkAlarm()` — Check if current time matches alarm time
- `triggerAlarm()` — Execute alarm notification
- `playAlarmSound()` — Generate and play audio alert

## License

Open source - feel free to use and modify as needed.

## Author

Created with Claude Code

---

**Note**: Make sure your browser has permission to play audio for the alarm sound to work properly.
