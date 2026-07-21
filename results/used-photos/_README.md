# Used Photo Compression Notes

This folder is a working copy of the still/photo assets currently used by the page.
It is for batch compression review only; the live page still references the original
paths in `public/hero`, `public/results/years`, and `public/results/posters`.

## Current Working Copy

The files in this folder have been converted to JPEG and aggressively compressed
for mobile review:

- Max image dimension: `640px`
- JPEG quality: `68`
- Intended target: low-bandwidth mobile film-reel display

## Recommended Targets

- Results film photos: keep around `640px` to `720px` wide for the mobile-only reel.
- Results film photo file size: aim for `35KB` to `90KB` each.
- Large PNG year images: convert to JPEG/WebP; target `50KB` to `100KB`.
- 2026 poster: current small source is already fine.

## Other Mobile Assets To Compress

- Hero video `public/hero/yy-lam-campaign-vertical.mp4`: current file is about `2.0MB`, `320x568`, `25.15s`.
  The size issue is bitrate/duration, not resolution. For mobile, target about `1.5MB` to `3MB`.
- YY Reads MP3 files in `public/audio/readings`: compressed from 128kbps stereo to 64kbps mono on 2026-07-19.
  Original files were backed up to `/Users/matthew/Desktop/yy-original-audio-readings-2026-07-19`.
- Paper background `public/results/paper-bg.jpg`: compressed to about `32KB`.
- Gold foil texture `public/textures/gold-foil.jpg`: compressed to about `52KB`.

## Practical Rule

The mobile canvas is at most `520px` CSS wide. The Results film cards render around
`172px` to `238px` CSS wide, so `640px` sources are enough for an intentionally
aggressive mobile compression pass.
