# sleapyTV Donate Component

A simple Twitch Extension component that displays a clickable donation banner link
link.

## Files

- `config.html` - the extension configuration page.
- `video_component.html` - the video component that displays the banner and opens the donation page.
- `donate_banner.jpg` - the banner background image.
- `sleapytv-donate.zip` - the extension package, if you are using the provided archive.

## Set Your Donation Link

Before uploading the files, open `video_component.html` and replace
`PLESE ADD YOUR DONATE LINK` with your donation URL. This placeholder appears
twice in the file; update both occurrences.

## Customize the Banner

Prepare if you will your own image with the exact filename `donate_banner.jpg`
and add it to the zip package, that goes to Twitch Developer Console. The
component references this filename, so do not rename it unless you also update
the image path in `video_component.html`.

## Configure in the Twitch Developer Console

1. Open the Twitch Developer Console and select your extension or create new
	one! - link to shor video with HOWTO:
2. ZIP all 3 files `confing.html` `video_component.html` `donate_banner.jpg`
3. Upload ZIPED package in your Twitch Dev Console
4. Save your changes and test the component in the extension preview. For more
	information please revisite HOWTO tutorial.

The component uses the Twitch Extension Helper:
`https://extension-files.twitch.tv/helper/v1/twitch-ext.min.js`.
