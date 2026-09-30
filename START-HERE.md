# Presenter - start here

**You do NOT need Command Prompt or `node server.js` any more.**

1. Install the Presenter desktop app (`Presenter-Setup.exe` from the GitHub Releases page,
   see BUILD-APP-ON-GITHUB.md). Open it - the phone connection starts by itself.
2. Install the phone app (`PresenterRemote.apk`) on your Android phone.
3. Open Presenter Remote on the phone (same Wi-Fi as the PC). It finds the computer on its own.
   The first time, a box appears on the PC: click **Allow**. That's the only step - after this the
   phone reconnects by itself every time.

iPhone: click **Phone** in the Presenter window on the PC and scan the QR code with the camera.

(Advanced: running `node server.js` still works, but then the phone asks for the PIN shown in that window.)

## OBS with a transparent background
In OBS add a **Browser Source** with the URL `http://localhost:8787/live` (Presenter must be open on the same computer).
It is transparent and follows your slides, font, colour and transition settings - no Live window needed.
(Window Capture also works: set Settings -> Display background -> Transparent, then tick **Allow Transparency**
in OBS's Window Capture properties.)
