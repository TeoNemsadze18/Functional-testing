# LIVE-SHR-002 - Clicking "Share" Menu During Live Stream Pauses Video and Triggers Reconnection

* **Severity:** Medium
* **Environment:** Android 14 · Red Note 14S · Staging · v1.23.0
* **Reproducibility:** 100%

## Summary
During an active live stream, tapping "Share" opens the share menu while automatically pausing the live video stream. Closing the share menu triggers a reconnection process that takes several seconds before the live stream resumes.

## Steps
1. Open the mobile application and join an active live stream.
2. Tap the "Share" button.
3. Observe the live video playback while the share menu is open.
4. Close the share menu.
5. Observe how the live stream recovers and resumes.

## Actual
Opening the "Share" menu pauses the live stream, and closing the menu triggers a reconnection ("Reconnect") requiring a delay of several seconds to restore the live stream.

## Expected
Opening the "Share" menu should keep the live stream running smoothly without pausing, and closing the menu should not require waiting for a reconnection.

## Notes
Subcategory: Functional Appropriateness / Correctness. Opening a native or in-app share sheet suspends media playback or network session state, causing a reconnect delay upon dismissal.
