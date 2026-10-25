# Splice

A small video editor for your phone. Trim clips, put them in order, and stitch them into one video. It runs entirely in the browser: clips never leave the device, and it works offline once installed.

**Use it:** https://fynhav.github.io/phone-video-editor/

## Install on iPhone

1. Open the link above in Safari.
2. Tap **Share → Add to Home Screen**.
3. Open Splice from the home screen. After the first launch it works without a connection.

## Editing

- **Add** clips from your camera roll (several at once is fine).
- **Scrub** by swiping the filmstrip; the line in the middle is the playhead. Pinch the strip to zoom.
- **Trim**: tap a clip, then drag the blue handles at either end.
- **Move**: hold a clip and drag it, or use the Earlier / Later buttons.
- **Split** cuts the clip under the playhead. **Copy** and **Delete** act on the selected clip.
- **Transitions**: tap the ⋈ marker between two clips. Choose Cut, Crossfade, Fade black, Fade white or Blur, and set the length. *Use on all cuts* copies it everywhere.
- **Stamp** burns the date, time or both into the top-left corner, in a camcorder or clean style. It reads when each clip was recorded from the video itself, and you can correct any time in the same sheet.
- **Canvas** sets the frame shape: original, 9:16, 1:1 or 16:9. Clips that don't match get bars, never cropped.
- **Save** joins the clips into one MP4. On iPhone, choose **Save Video** in the share sheet to put it in Photos.

## Saving your edit

Splice saves your edit automatically on the phone after every change: clip order, trims, transitions, stamp, frame shape and small strip images, usually well under 1 MB. It doesn't copy your videos.

A web app can't reopen videos from Photos on its own later, so when you come back Splice shows your timeline and lists the clips it needs. Tap **Re-select clips** and pick them, all at once and in any order. Each one is matched back to its place by length, size, recording date and name. Any video that isn't part of the edit is added at the end.

## Notes

- Joining runs at playback speed, so a 90-second edit takes about 90 seconds. Keep the screen awake while it works.
- No build step: `index.html`, `sw.js` and `manifest.webmanifest` are the whole app. When you change `index.html`, bump `VERSION` in `sw.js` so installed copies pick up the update.
