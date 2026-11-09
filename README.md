<div align="center">

# 🌙 Nocturne

### Your Music. Your Mood. Your Space.

A modern, browser-based music discovery and listening experience.

![Status](https://img.shields.io/badge/status-in%20development-yellow?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-web-blue?style=for-the-badge)
![Built with](https://img.shields.io/badge/built%20with-HTML%20%7C%20CSS%20%7C%20JavaScript-orange?style=for-the-badge)
![Music source](https://img.shields.io/badge/primary%20music%20source-Audius-purple?style=for-the-badge)

</div>

---

## About

**Nocturne** is an independent web application project exploring a more personal way to discover and listen to music. It brings music discovery, playback controls, saved tracks and customisable interfaces into one browser-based experience.

Audius is the primary online music source. The project is designed with a multi-source approach so that additional music catalogues can be considered over time, subject to their APIs, playback rules and licensing.

Nocturne is currently an experimental project under active development.

## Features

- **Online music discovery** — discover and search tracks available through supported music sources.
- **Audius integration** — primary provider for music discovery and streaming of available tracks.
- **Music player** — playback controls including play, pause, next, previous, shuffle, repeat, volume and seeking, where supported by the source.
- **Personal library** — save tracks and keep library information in browser storage.
- **Mood-based discovery** — select a mood to influence music suggestions.
- **Five interface styles** — switch between different visual experiences.
- **Responsive layout** — designed for desktop and mobile browser screens.
- **Local music support** — import audio files from your device for local playback.

## Interface styles

| Style | Design direction |
| --- | --- |
| **Olive Pulse** | Dark, immersive and mood-focused |
| **Minimalist** | Clean, simple and spacious |
| **Atlas** | Editorial-inspired discovery layout |
| **Horizon** | Cinematic and atmospheric |
| **Studio** | Playback-focused visual design |

## Technology

- HTML5
- CSS3
- JavaScript
- Audius API
- IndexedDB
- LocalStorage
- Progressive Web App foundations (manifest and service worker)

## Getting started

### Requirements

- A modern web browser
- An internet connection for online music discovery and streaming
- Visual Studio Code (recommended)
- The Live Server extension for local development

### Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/imSaikrishn/nocturne-music.git
   ```

2. Open the project folder:

   ```bash
   cd nocturne-music
   ```

3. Open the folder in Visual Studio Code.
4. Install the **Live Server** extension if it is not already installed.
5. Open `index.html`.
6. Right-click in the editor and select **Open with Live Server**, or click **Go Live** in the status bar.
7. Your browser should open the local Nocturne site.

> Use the local development server rather than opening `index.html` directly. Some browser features, including service workers, require a secure context such as `localhost` or HTTPS.

## Project structure

```text
nocturne-music/
├── index.html
├── styles.css
├── app.js
├── manifest.webmanifest
├── sw.js
├── icon.svg
└── README.md
```

## Music sources and availability

Audius is Nocturne's primary music provider. Search results and playback depend on what Audius makes available for a track and whether its service is reachable.

The catalogue does not include every commercial release. Some tracks may be unavailable, restricted, removed or unable to stream. Nocturne does not bypass provider restrictions or extract audio from third-party services.

Additional providers may be added only through their permitted APIs, official players or other authorised playback methods.

## Privacy

Nocturne is designed as a browser-first project.

- Saved library information and preferences are stored in browser storage.
- Imported audio files are kept in the browser's local storage database.
- Music discovery and streaming requests are sent to the relevant external music provider.
- Clearing browser site data may remove locally saved information and imported files.

This prototype does not currently provide cloud synchronisation or account-based backup.

## Roadmap

- [x] Initial browser-based application
- [x] Five interface style concepts
- [x] Audius as the primary music source
- [x] Local music import and playback foundation
- [x] Browser-based saved library foundation
- [ ] Verify reliable live streaming across different Audius tracks
- [ ] Improve search quality and Indian-language discovery
- [ ] Improve recommendations using listening preferences
- [ ] Expand playlist creation and management
- [ ] Add more authorised music providers
- [ ] Complete accessibility and cross-browser testing
- [ ] Develop an Android version after the web experience is stable

## Contributing

Nocturne is a work in progress. Suggestions, bug reports and thoughtful contributions are welcome.

If you find a problem:

1. Check whether it has already been reported.
2. Open an issue with steps to reproduce it.
3. Include your browser and operating system.
4. Attach relevant screenshots or console errors, but do not share private API keys or personal data.

Pull requests should explain the change and include relevant testing details.

## Copyright and disclaimer

Nocturne is an independent project and is not affiliated with or endorsed by Audius or any other music provider.

Nocturne does not claim ownership of music, artwork or metadata supplied by external services. Such content remains the property of its respective owners and is subject to the relevant provider terms, copyright and licensing conditions.

## Project status

Nocturne is an **experimental project under active development**. Features and integrations may change. Online playback depends on third-party service availability, track permissions, network conditions and browser support. Not every feature has been verified across all browsers and devices.

---

<div align="center">

**NOCTURNE**

*Your Music. Your Mood. Your Space.*

Created by [@imSaikrishn](https://github.com/imSaikrishn)

</div>
