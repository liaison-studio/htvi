# Troubleshooting — Head Tracker+Voice+Instructor

🌐 English · [Русский](troubleshooting.ru.md) · [Français](troubleshooting.fr.md) · [Deutsch](troubleshooting.de.md) · [Italiano](troubleshooting.it.md)

Find your symptom, then follow the steps in order. If nothing helps, [send a report](#send-a-report-to-the-developer).

## Installation

### "Windows protected your PC" — no way to continue
Click **More info**, then **Run anyway**. If there is no **Run anyway** button, Smart App Control is on: see [Installation, step 2.5](install.en.md).

### The browser refuses to keep the downloaded file
Edge: **…** → **Keep** → **Show more** → **Keep anyway**. Chrome: click the file → **Download unsafe file**.

### The first start takes a long time
Microsoft Defender scans the new program; it can take up to a minute. Wait.

### The setup says "The program is running: close it…"
Close the program with **File → Exit** (not only the window's ✕), then run the setup again.

## iPhone connection

### The iPhone app says there is no connection to the PC
1. The PC program must be running.
2. **Cable:** plug it in, unlock the iPhone, and answer **Trust** if it asks "Trust this computer?".
3. **Wi-Fi:** the PC and the iPhone must be on the same network.
4. Tap **Retry** in the app.

### The connection worked, then stopped during the flight
1. Check the cable (or the Wi-Fi).
2. Click **Start** again in the PC program.
3. If the app shows a weak Wi-Fi quality, use the cable or move closer to the router.

### The iPhone looks fine, but the PC says "face not visible"
1. In the PC program, open **Settings → iPhone** and choose the connection (cable or Wi-Fi) again.
2. Click **Start** again.

### With the cable, the iPhone is sometimes not found
1. Unplug and plug the cable back in, with the iPhone unlocked.
2. Close other programs that use the iPhone as a camera or webcam.
3. Try another cable or another port of the PC.

## Head tracking

### The view does not move
1. At the bottom of the main window: is **RUNNING** shown in green? If not, click **Start**.
2. In the View block: does it say **face visible**? If not, see below.
3. Sit straight and click **Center** (Ctrl+Alt+C).
4. Check that **Pause** is not on (Ctrl+Alt+X switches it).

### "Face not visible"
- The iPhone must face you, about an arm's length away, without anything between you and the camera.
- Avoid a strong light directly behind your head.
- If you covered your face for a moment, tracking comes back by itself after a few seconds.

### The view is slow, jerky or too sensitive
**Profiles → View settings** → click the ready-made curve **Fighter** or **Civil**. Then fine-tune **Sensitivity** and **Smoothing** in the main window.

### The view goes the wrong way (left instead of right)
Open **Profiles → View settings**. In the **Axes** list, click the ⇄ icon to the right of that axis (⇄ = inverted). Then please [report it](https://github.com/liaison-studio/htvi/issues/new/choose) with the name of the simulator: the direction should be right without changes.

### The view drifts off-center over time
Sit straight and press **Ctrl+Alt+C** (or say "center the view"). To correct it automatically, turn on **Slow auto-recenter** in **Profiles → View settings**.

## Voice commands

### A command is not recognized
1. The command language in the PC program (**Settings → Voice**) and the speech language on the iPhone (**Settings → Speech language**) must be the same. If they differ, the main window shows a yellow banner.
2. If PTT is used, hold the button while you speak.
3. Speak briefly, like a pilot: "gear down", not a long sentence.
4. The list of phrases for your game is in the **Commands** window.

### A command was recognized but did nothing in the game
Click **Didn't work — disable** under the last command. The program notes it so the command can be fixed. Please also [report it](https://github.com/liaison-studio/htvi/issues/new/choose) with the phrase and the simulator.

## Instructor

### The instructor is silent
Windows has no voice for your language. **Windows Settings → Time & language → Speech → Add voices**, add a voice for your language, then restart the program.

### The instructor follows the wrong aircraft
In the Instructor block, choose the aircraft yourself instead of **Auto**.

## Send a report to the developer
1. **Service → Report for the developer…**
2. Describe what happened.
3. Click **Save the archive…**. The archive is saved in *Documents → Head Tracker Voice Instructor → Reports*.
4. Attach it to a [bug report](https://github.com/liaison-studio/htvi/issues/new/choose) or send it to liaison.studio.contact@gmail.com.

The report contains no audio and no pairing data. The program never sends anything by itself.
