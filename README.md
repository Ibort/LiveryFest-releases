# MotoLivery — downloads

Two Windows programs for The Crew Motorfest. **MotoMaker** turns a picture into a design
file. **MotoLivery** takes a design file and builds it in the game's livery editor for you,
by driving the controller through a PS5 stream.

This repository carries the downloads and nothing else. The source lives in a separate
private repository.

## Downloads

1. Open the [Releases page](https://github.com/Ibort/liveryfest-releases/releases).
2. On the newest release, download the `MotoLivery-<version>.zip` file listed under
   **Assets**. It is about 70 MB.
3. Unzip it to **Documents** or your **Desktop** — not to Program Files.
4. Double-click `MotoLivery.exe` to build a design, or `MotoMaker.exe` to make one.

You do not need a GitHub account, and nothing is installed: both programs run out of the
folder you unzipped, and deleting the folder removes them completely.

Windows only. Windows may say *"Windows protected your PC"* the first time — that is
SmartScreen not recognising a small program nobody has paid to sign. Click **More info**,
then **Run anyway**.

## Updating

Delete the old folder and unzip the new one. You do not have to set anything up again:
your calibration, your settings and your designs live in `%LOCALAPPDATA%\MotoLivery` under
your user folder, not in the app folder, precisely so an update cannot take them with it.

## How you will know there is a new version

Both programs check for themselves. When a window opens, and at most once every 24 hours,
the app makes one request to GitHub asking for the newest release here. If that release's
tag is a higher version number than the copy you are running, a green bar appears across
the top of the window saying `Version 0.9.2 is out — you have 0.9.1`, with three buttons:

* **what's new** opens that release's page in your browser.
* **skip this version** never mentions that particular version again. The next one after
  it is a different version, so it will still be offered.
* **✕** closes the bar for now.

Nothing is downloaded and nothing is installed — the bar is a sentence and three buttons,
and you still fetch the zip yourself from the Releases page.

The check sends nothing but the request: no account, no sign-in, no telemetry. If it
cannot reach GitHub, or there is no newer release, it says nothing at all rather than
interrupting you to report that it could not check.

MotoMaker also has a **Check for updates** button, which just opens the Releases page in
your browser.
