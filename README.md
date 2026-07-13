[README.txt](https://github.com/user-attachments/files/29949583/README.txt)
ANODIZE INSPECTOR — SETUP GUIDE
================================
Everything runs 100% offline, on-device. No internet or install required
to use it — the options below just control whether it opens as a normal
browser tab or as its own standalone app window/icon.


WINDOWS DESKTOP
---------------
Easiest path (no window chrome, no server needed):
 1. Double-click index.html to open it in your browser.
 2. Click the three-dot menu (Chrome/Edge) -> "Cast, save, and share" or
    "More tools" -> "Create shortcut..."
 3. Check "Open as window" -> Create.
 4. A desktop icon now launches the app in its own window, no address
    bar or tabs — just like a normal installed program.

Full PWA install (adds it to Start Menu, works the same way):
 1. Double-click "Start Inspector (Windows).bat" (requires Python,
    which most Windows PCs used for QA/engineering already have).
 2. Your browser opens the app at http://localhost:8743
 3. Click the "Install App" button in the app's header (top right),
    or the install icon in the browser's address bar.
 4. It's now a standalone app you can pin to the Start Menu/taskbar.


iPHONE / iPAD (iOS)
--------------------
 1. AirDrop, email, or copy the whole "app" folder onto the device
    (or place it in the Files app / iCloud Drive).
 2. Open index.html in Safari (must be Safari, not Chrome, for this step).
 3. Tap the Share icon -> "Add to Home Screen" -> Add.
 4. A full-screen app icon now appears on the home screen — it opens
    without Safari's address bar, like a real app.
 Camera access for live capture works the same as in Safari.


ANDROID PHONE / TABLET
-----------------------
Local file (simplest, opens with Chrome's browser bar visible):
 1. Copy the "app" folder onto the device.
 2. Open index.html in Chrome.
 3. Menu -> "Add to Home screen."

Full standalone app window (no browser bar) — requires a local server,
same as Windows:
 1. If your inspection PC and phone share the same Wi-Fi/LAN, run
    "Start Inspector (Windows).bat" on the PC.
 2. On the phone, open Chrome and go to: http://<PC's local IP>:8743
    (find the PC's IP with "ipconfig" in Command Prompt, e.g. 192.168.1.20)
 3. Menu -> "Install app" (Chrome will offer this once the page loads
    correctly from that address).


NOTES
-----
- The sample library and zone templates are saved by the browser you
  use, tied to that browser + device. They do not sync between devices —
  use the "Export Library" / "Import Library" buttons in the app to move
  your taught samples between machines.
- No data ever leaves the device; there is no cloud, account, or network
  requirement for the app to function.
