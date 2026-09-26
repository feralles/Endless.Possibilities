# Sleapytv Link Twitch Extension

This package contains the Twitch Extension files for the broadcaster configuration page and stream overlay.

## Included files

- sleapytv-link/config.html
- sleapytv-link/video_overlay.html

## What this extension does

- allows the broadcaster to configure a list of action buttons
- supports custom links and integration-style buttons
- renders a modular overlay on stream
- uses the Twitch extension helper API and broadcaster configuration storage

## Recommended Twitch setup

1. Open the Twitch Developer Console.
2. Create or edit a Twitch Extension.
3. Upload the files as your extension frontend pages.
4. Use the following page mappings:
   - Config page: config.html
   - Overlay page: video_overlay.html
5. In the extension panel, set the proper config page and overlay URL values.

## Important notes

- The extension relies on the Twitch helper script:
  https://extension-files.twitch.tv/helper/v1/twitch-ext.min.js
- The config is saved in the broadcaster configuration area using the Twitch extension configuration API.
- The overlay is generated dynamically from the saved config.
- If the backend endpoint or auth data is not available, the code gracefully falls back to the button URL when possible.

## Runtime safety

The current version includes basic guards for:
- missing config
- malformed JSON
- missing auth token
- missing button URL
- empty or invalid values

This helps avoid hard crashes in the Twitch extension runtime.

## File structure

```text
.
├── README.md
├── sleapytv-link/
│   ├── config.html
│   └── video_overlay.html
└── package zip generated separately
```

## Deployment reminder

Keep the file names as-is unless you also update the Twitch extension configuration to match the new names.

## Support

This is a starter/functional build for extension configuration and overlay presentation. It is intended to be adjusted for your final backend integration and branding.
