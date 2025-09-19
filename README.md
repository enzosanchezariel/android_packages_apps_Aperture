# LineageOS 20 Aperture Camera FIX

This repository fixes all the UI issues in the LineageOS 20 camera app, Aperture.
The LineageOS development team only focuses on bug fixes in their most recent versions, which leaves unofficial builds and other ROMs/GSIs based on earlier releases stuck with these issues.

## Fixes included
- Google Lens button overlapping with the zoom slider in camera SCAN mode.
- Invisible "retry" and "accept" buttons in singleCaptureMode.
- Camera mode background chip visible in singleCaptureMode.
- Ability to slide into another camera mode while in singleCaptureMode.

## About singleCaptureMode
singleCaptureMode is the mode used when any app requests a photo or video from the system camera through the intents android.media.action.VIDEO_CAPTURE and android.media.action.IMAGE_CAPTURE.
Since Android 10, only the system camera(s) can handle these intents.

## Testing tool
To test these intents, I created a simple app with two buttons: one for a video intent and one for a photo intent. You can find this app in the release 2.0 files.
Make sure to grant camera permission first, otherwise the app will crash.
