# DevSurf releases

Windows installer and portable downloads for **Devsurf**.

## Download

Download [Devsurf Setup 1.3.1](https://github.com/GianCarlozxc/DevSurfRelease/releases/download/v1.3.1/Devsurf-Setup-1.3.1.exe) and run it. Setup installs the app and creates a desktop shortcut named **Devsurf**, without `.exe` in the desktop label. No extraction is needed.

The [latest release](https://github.com/GianCarlozxc/DevSurfRelease/releases/latest) also provides an optional portable ZIP used by the in-app updater. **SHA256SUMS.txt** covers both downloads.

## AI setup

Public builds contain no developer API keys or personal browser data. Groq chat connects automatically through the hosted DevSurf AI service without a user API key. Messages pass through DevSurf AI to Groq; shared usage limits apply. Alternatively, use your own `GROQ_API_KEY` or run Ollama locally and select an installed model. Free AI Horde image generation is subject to service availability and queues.


## Update inside DevSurf

Starting with v1.1.0, go to **Settings > About DevSurf > Check for updates**, then select **Update and restart**. Downloads, verification and installation happen inside the app, followed by an automatic restart. Browser profiles and local AI configuration are preserved. The previous installation is restored if the replacement fails to start.

v1.0.0 users need to download the latest release once to get the updater. Future stable releases use the in-app update flow; prereleases and older versions are ignored.

If an older build remains open after downloading an update, install v1.3.1 manually once. It fixes the Windows helper lifetime and update shutdown; future in-app updates restart the new version automatically.
