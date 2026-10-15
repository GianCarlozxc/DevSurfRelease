# DevSurf releases

Windows installer and portable downloads for **Devsurf**.

## Download

Download [Devsurf Setup 1.6.0](https://github.com/GianCarlozxc/DevSurfRelease/releases/download/v1.6.0/Devsurf-Setup-1.6.0.exe) and run it. Setup installs the app and creates a desktop shortcut named **Devsurf**, without `.exe` in the desktop label. No extraction is needed.

The [latest release](https://github.com/GianCarlozxc/DevSurfRelease/releases/latest) also provides an optional portable ZIP used by the in-app updater. **SHA256SUMS.txt** covers both downloads.

## AI setup

Public builds contain no developer API keys or personal browser data. Groq chat connects automatically through the hosted DevSurf AI service without a user API key. Messages pass through DevSurf AI to Groq; shared usage limits apply. Alternatively, use your own `GROQ_API_KEY` or run Ollama locally and select an installed model. Free AI Horde image generation is subject to service availability and queues.


## Update inside DevSurf

Starting with v1.1.0, go to **Settings > About DevSurf > Check for updates**, then select **Update and restart**. Downloads, verification and installation happen inside the app, followed by an automatic restart. Browser profiles and local AI configuration are preserved. The previous installation is restored if the replacement fails to start.

v1.0.0 users need to download the latest release once to get the updater. Future stable releases use the in-app update flow; prereleases and older versions are ignored.

If an older build remains open after downloading an update, install v1.4.0 manually once. It fixes the Windows helper lifetime and update shutdown; future in-app updates restart the new version automatically.

DevSurf 1.4.0 adds website isolation hardening, HTTPS-first, site-data clearing and risky-download warnings. Future updates require an Ed25519-signed update-manifest.json verified against the public key pinned in the app, alongside SHA-256 checks. Versions before 1.4.0 do not enforce this signature policy. Install the trusted initial 1.4.0 build to establish the pinned key. Windows publisher signing is separate and remains unconfigured; the EXE is not Authenticode-signed. Anonymous AI retains shared service limits.

Version 1.4.1 fixes staging failures caused by Electron treating its demo .asar archive as a virtual directory. New downloads omit the unused archive so older updaters can install this version too. Check again for 1.4.1 and leave the browser open through verification, unpacking and preparation until it restarts.

Version 1.5.0 adds five free-eligible LLM7 text models. LLM7 credentials are protected with Windows account encryption outside the installation and are not bundled in downloads. The LLM7 model group appears only on Windows accounts configured with their own key; hosted Groq continues to work for public users. Provider quotas and terms apply.

Version 1.6.0 adds Gemini 3.8 Flash, Gemini 3.5 Flash-Lite and Gemini 3.1 Flash-Lite through Google AI Studio. Keys stay encrypted on the configured Windows account and are excluded from downloads. Google free-tier quotas, project billing settings and data-use terms apply. Paid Google models/tools are not enabled.
