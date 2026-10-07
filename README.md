# LiveryFest — downloads

LiveryFest turns a picture into a livery for The Crew Motorfest and builds it in the game's
livery editor for you. One Windows program, `LiveryFest.exe`, opens its three parts:

* the **Maker** turns a picture into a design;
* the **Builder** builds a design in the game by driving the controller, on a PS5 through a
  chiaki-ng stream or in the PC game;
* the **Designer** lets you draw or correct a design by hand in your browser.

This repository carries the downloads and nothing else. The source lives in a separate
private repository.

## Downloads

1. Open the [Releases page](https://github.com/Ibort/liveryfest-releases/releases).
2. On the newest release, download the `LiveryFest-<version>.zip` file listed under
   **Assets**. It is about 70 MB.
3. Unzip it to **Documents** or your **Desktop** — not to Program Files.
4. Double-click `LiveryFest.exe`. It asks whether you want the Maker (make a design from a
   picture), the Builder (build a design in the game) or the Designer (draw one by hand).

You do not need a GitHub account, and nothing is installed: everything runs out of the
folder you unzipped, and deleting the folder removes them completely.

Windows only. Windows may say *"Windows protected your PC"* the first time — that is
SmartScreen not recognising a small program nobody has paid to sign. Click **More info**,
then **Run anyway**.

## Updating

Delete the old folder and unzip the new one. Unzipping over the old folder can leave old
files behind, such as `LiveryFest-Maker.exe` from 0.9.5 and earlier. You do not have to
calibrate again: your calibration, your settings and your designs live in
`%LOCALAPPDATA%\LiveryFest` under your user folder, not in the app folder, precisely so an
update cannot take them with it.

If you build in the PC game, tell the Builder once more which game you drive: press
**Set up…**, then **Choose** beside "Which game are you driving?". Tick **Motorfest installed
on this PC**, click the game's window in the list and press **Save**. Then close the Builder
and open it again while the game is running, so it puts your window size back. That one
choice is kept in the app folder, so a new copy starts on the PS5.

## How you will know there is a new version

The Maker and the Builder check for themselves. When either window opens, and at most
once every 24 hours, the app makes one request to GitHub asking for the newest release here.
If that release's tag is a higher version number than the copy you are running, a green bar
appears across the top of the window saying `Version 0.10.0 is out — you have 0.9.5.`, with three buttons:

* **what's new** opens that release's page in your browser.
* **skip this version** never mentions that particular version again. The next one after
  it is a different version, so it will still be offered.
* **✕** closes the bar for now.

Nothing is downloaded and nothing is installed — the bar is a sentence and three buttons,
and you still fetch the zip yourself from the Releases page.

The check sends nothing but the request: no account, no sign-in, no telemetry. If it
cannot reach GitHub, or there is no newer release, it says nothing at all rather than
interrupting you to report that it could not check.

The Maker, and the Builder's Simple face, also have a **Check for updates** button, which
just opens the Releases page in your browser.
