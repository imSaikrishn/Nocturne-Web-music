# Nocturne — Audius-first Web Music Player

A browser-based music player with Audius as its primary online catalogue. You do not need MP3 files, a paid API plan, or a YouTube API key to use the basic Audius search and streaming features.

## Run locally
1. Extract the project.
2. Open the folder in VS Code.
3. Start the folder with Live Server, or run `python -m http.server 8000` in this folder.
4. Visit `http://localhost:8000`.

Use localhost or HTTPS. Browser storage, service workers and some media features may not work when opening the HTML file directly with `file://`. Internet access is required for Audius music.

## Audius-first features
- Trending tracks loaded on Home.
- Search tracks by title, artist, or keywords.
- Stream full tracks when the Audius track is marked streamable and the source is available.
- Save Audius tracks to the browser library without downloading audio.
- Previous/next, shuffle, repeat, volume and seek controls.
- Five interface styles: Olive Pulse, Minimalist, Atlas, Horizon and Studio.
- Local listening preference storage and simple mood keyword sorting.
- Automatic fallback between Audius public discovery API nodes.

## Important catalogue limits
Audius is an open music catalogue, not a licensed copy of every commercial streaming catalogue. It is strongest for independent and creator-published music. Mainstream releases may be missing, region-restricted, unavailable, or not streamable. No legal source can guarantee every song worldwide.

## API and cost
The app uses Audius public read-only endpoints and sends an `app_name=Nocturne` query parameter. Audius documents that most read-only endpoints work without credentials; an API key is for higher rate limits. This project does not require purchasing an API key for basic use. If usage grows, register an app and follow Audius rate-limit guidance.

## Privacy
Saved track metadata, theme preference and listening signals are stored in this browser. Audio is streamed, not downloaded into the library. Clearing site data removes local preferences and saved-library entries.

## Verification notes
- JavaScript syntax check: passed with Node.js.
- Static HTML checks: no duplicate element IDs and no missing static IDs referenced by the app.
- All five theme buttons and their theme selectors are present.
- Automated browser interaction and live Audius streaming could not be completed in this build environment because browser navigation and outbound DNS/network requests are blocked here. Test on your own browser with an internet connection before treating this as release-ready.

## Not yet implemented
- Audius account sign-in and cloud-synced favorites/playlists.
- Robust AI recommendations; current mood sorting uses simple metadata keywords.
- Guaranteed background playback on every browser/device.
- Complete commercial catalogue coverage.
- Android APK packaging; validate this web build first.

Audius API docs: https://docs.audius.co/api/


## Expanded Indian music discovery
- Audius remains the primary full-track streaming source where tracks are available.
- Deezer and Apple Music/iTunes catalogue search add Indian and international discovery with short previews where supplied. Deezer search currently uses a public CORS relay; availability and rate limits may vary.
- JioSaavn results are opened on JioSaavn's official website. No unofficial stream extraction is used. Full-song playback is controlled by JioSaavn and may depend on region/account rules.
- Catalogue search is not a promise that every track has a playable preview or full stream.
