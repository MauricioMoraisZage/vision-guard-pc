# Changelog

All notable changes to Vision Guard PC will be documented in this file.

This project follows [Semantic Versioning](https://semver.org/):

* **MAJOR** version for incompatible or substantial product changes;
* **MINOR** version for new backward-compatible features;
* **PATCH** version for backward-compatible bug fixes.

---

## [Unreleased]

No unreleased changes.

---

## [1.0.1] — 2026-07-06

### Added

- Clickable technical support email in the application interface.
- Startup and runtime logging for troubleshooting.

### Fixed

- Improved Windows autostart reliability by copying the executable to a stable location within the user's local application data directory.
- Automatic repair of outdated Windows startup registry entries.
- Delayed system tray initialisation during Windows sign-in.
- Verification that the system tray icon is ready before completing startup.

---

## [1.0.0] — 2026-07-05

### Added

* Native Windows desktop application for healthier computer-use habits
* Active screen-time tracking
* Inactivity detection based on mouse and keyboard interaction
* Configurable blink reminders
* Configurable visual breaks
* Configurable physical breaks
* Daily computer-use limit
* Nighttime usage lock
* Focus Mode with the following durations:

  * 30 minutes
  * 45 minutes
  * 1 hour
  * 2 hours
* Entertainment Mode with the following durations:

  * 1 hour
  * 2 hours
  * 2 hours and 30 minutes
  * 3 hours
* Non-blocking wellness notifications during long entertainment sessions
* Usage statistics
* Local SQLite persistence
* Portuguese and English interfaces
* Persistent language preference
* Persistent wellness settings
* Persistent main-window size, position, and maximized state
* Responsive main dashboard
* Responsive Settings and Statistics windows
* Responsive visual and physical break screens
* Automatic scrollbars that appear only when required
* Mouse-wheel scrolling across the main interface
* Windows system tray integration
* Optional startup with Windows
* Single-instance application protection
* Local application-data storage
* Author credits and application version information
* Windows executable generation support
* Automated unit tests
* Project verification script

### Changed

* Improved wording for inactivity and physical-break status
* Changed the physical-break status label to “No physical break for”
* Improved Portuguese interface translations
* Improved window navigation to behave like a native desktop application
* Settings and Statistics now inherit the size and state of the main window
* The main window now opens centered on the first execution
* The application now restores the user’s previous window state
* Reduced the minimum supported main-window size to `760 × 520`
* Improved responsive layout for Focus Mode and Entertainment Mode controls
* Updated default nighttime lock schedule:

  * starts at `22:30`
  * ends at `07:30`
* Updated default daily usage limit to 10 hours
* Updated default inactivity threshold to 10 minutes

### Fixed

* Fixed incomplete Portuguese translations on the main dashboard
* Fixed uppercase dashboard labels not being translated
* Fixed saved settings not appearing correctly when reopening Settings
* Fixed Settings callback parameter mismatches
* Fixed oversized input fields in Settings
* Fixed buttons being cut off on smaller windows
* Fixed mouse-wheel scrolling requiring the pointer to be over the scrollbar
* Fixed secondary windows opening behind the Windows taskbar
* Fixed secondary windows not matching the main-window state
* Fixed windows occasionally becoming invisible during navigation effects
* Removed slow and inconsistent fade transitions
* Fixed Entertainment Mode test-file indentation
* Fixed Entertainment Mode inactivity handling for films and videos
* Fixed physical-break and inactivity status semantics
* Fixed window-state restoration on smaller displays

### Security and privacy

* Application data remains stored locally
* No user account is required
* No advertising or third-party telemetry is included
* Typed content, passwords, websites, documents, camera, and microphone data are not monitored

---


## Versioning guide

Examples of future versions:

| Version | Meaning                               |
| ------- | ------------------------------------- |
| `1.0.1` | Bug fix                               |
| `1.1.0` | New backward-compatible feature       |
| `2.0.0` | Major product or compatibility change |

---

## Planned

### Windows

* Microsoft Store distribution
* Signed Windows package
* Improved installer and update experience
* Additional accessibility options

### macOS

* Native inactivity detection
* Startup integration
* Menu-bar integration
* macOS application packaging
* Intel and Apple Silicon validation

### Linux

* Support for major desktop environments
* Idle-time detection for supported display servers
* Startup integration
* System-tray compatibility
* Linux application packaging

No macOS or Linux build will be published before being tested on the corresponding operating system.
