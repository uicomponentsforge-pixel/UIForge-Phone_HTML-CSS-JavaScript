# UIForge Phone - Web Edition

UIForge Phone - Web Edition is a web-based smartphone operating system simulation built using modern vanilla JavaScript (ES Modules), HTML5, and CSS3. It delivers an interactive mobile OS experience directly inside any modern browser.

## Features

- **System Shell & Interface**:
  - **Status Bar**: Live clock, battery status, Wi-Fi, and network icons.
  - **Navigation Bar**: Functional Home, Back, and Recents buttons.
  - **Notification Shade & Quick Toggles**: Swipe or click pull-down panel with Wi-Fi, Bluetooth, Flashlight, Dark Mode, Volume/Brightness sliders, and system notifications.
  - **App Drawer & Home Screen**: App launcher with search functionality.
  - **Lock Screen**: Swipe or tap to unlock device simulation.

- **Built-in Applications**:
  - 📞 **Phone**: Interactive dialer keypad and call logs.
  - 💬 **Messages**: Message threads and SMS interface.
  - 👤 **Contacts**: Contact management with persistent local storage.
  - 📷 **Camera**: Live webcam preview support using `getUserMedia`.
  - 🖼️ **Gallery**: Photo and media browser.
  - 🧮 **Calculator**: Functional standard calculator.
  - 📅 **Calendar**: Monthly view calendar with date tracking.
  - ⏰ **Clock**: Multi-functional clock with Alarm, World Clock, Stopwatch, and Timer.
  - 🎵 **Music**: Audio player interface with playback controls.
  - 🌤️ **Weather**: Live weather forecast powered by Open-Meteo API.
  - ⚙️ **Settings**: Device preferences including Dark Mode toggle, Volume/Brightness controls, and Wallpaper selection.
  - 📁 **Files**: Virtual file manager.
  - 🌐 **Browser**: Simulated web browser experience.

## Technology Stack

- **Frontend**: HTML5, Modern CSS3 (Variables, Flexbox, Grid, Glassmorphism design), Vanilla JavaScript (ES6 Modules).
- **State Management**: Reactive state observer (Pub/Sub pattern).
- **Storage**: `localStorage` API for saving user settings, contacts, and state.
- **External APIs**: Open-Meteo API for real-time weather updates.

## Repository Structure

```
├── index.html        # Main HTML entry point
├── css/
│   └── style.css     # Global styles and OS components styling
├── js/
│   ├── app.js        # Main entry point and OS initialization
│   ├── state.js      # Global state observer and OS event handler
│   ├── apps/         # Individual application implementations
│   ├── components/   # UI components (System Shell, Navigation, Notifications)
│   ├── services/     # Web APIs and background services (Weather, Audio, Device)
│   └── storage/      # LocalStorage utility wrapper
└── assets/           # Wallpapers and app icons
```

## Getting Started

No build tools or backend servers are required to run UIForge Phone.

### Quick Start

1. Clone or download the repository.
2. Open `index.html` directly in any modern web browser (Google Chrome, Mozilla Firefox, Safari, Edge).

### Running with a Local Server (Optional)

To serve the project over HTTP/HTTPS (recommended for ES module loading across all browsers):

Using Python:
```bash
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000` in your web browser.

Using Node.js (`serve` or `http-server`):
```bash
npx http-server .
```

## License

This project is open source and available under the standard project permissions.
