# DevSurf releases

Windows portable downloads for **DevSurf**.

## Download

Open the [latest release](https://github.com/GianCarlozxc/DevSurfRelease/releases/latest), download the Windows x64 ZIP, extract the entire folder, then run **DevSurf.exe**. Keep all extracted files together. Verify the ZIP using the accompanying **SHA256SUMS.txt**.

## AI setup

Public builds contain no developer API keys or personal browser data. For Groq chat, set your own `GROQ_API_KEY` environment variable before launching. Alternatively, run Ollama locally and select an installed model. Free AI Horde image generation is subject to service availability and queues.

## Source

The source code is maintained in [GianCarlozxc/Devsurf](https://github.com/GianCarlozxc/Devsurf), a private repository that requires access. This repository hosts downloadable builds and release notes. Third-party notices and component source references are included in each download.

## Update inside DevSurf

Starting with v1.1.0, go to **Settings > About DevSurf > Check for updates**, then select **Update and restart**. Downloads, verification and installation happen inside the app, followed by an automatic restart. Browser profiles and local AI configuration are preserved. The previous installation is restored if the replacement fails to start.

v1.0.0 users need to download v1.1.0 once to get the updater. Future stable releases use the in-app update flow; prereleases and older versions are ignored.
