# Reel Radar

Every movie and show you own in one library: what's on your Plex and Jellyfin servers and what you bought
digitally, with each copy's source and resolution, favorites and ranks. From [Blinken Labs](https://blinken-labs.com).

This repository holds the downloads only; the source code isn't published.

## Download

Get the [latest release](https://github.com/blinken-labs/ReelRadar-Releases/releases/latest). The app comes as a
disk image (`.dmg`) or a zip; either works.

macOS 15 (Sequoia) or later, on Apple silicon or Intel. Releases are signed with a Developer ID and notarized by
Apple. Reel Radar is in beta.

## Install and set up

1. Open the `.dmg` and drag Reel Radar onto Applications (or unzip and move it there), then open it.
2. Open **Sources** and choose **Plex** or **Jellyfin**. Click **Scan Network** to find your server, or type its
   address, then enter its **Plex Token** or Jellyfin **API Key**.
3. Choose the libraries to include and click **Sync Library**.
4. Optional: choose **Digital** to import a CSV list of the movies you own digitally. The file needs a **Title**
   column and an **IMDb ID** column; other columns are ignored. Enter your own free
   [TMDB](https://www.themoviedb.org) key there too, to fetch posters and descriptions.

On first launch macOS asks whether Reel Radar may find devices on your local network: choose **Allow**, or
Scan Network can't find your servers.

## If Scan Network finds nothing

You can always type the server's address instead: for example `http://192.168.1.10:32400` for Plex or
`http://192.168.1.10:8096` for Jellyfin.

- Check Reel Radar is turned on under System Settings, Privacy & Security, Local Network.
- If it isn't listed there and macOS never asked (a macOS 27 bug), quit Reel Radar, run
  `tccutil reset All com.blinkenlabs.ReelRadar` in Terminal, move every copy of Reel Radar to the Trash and empty
  it, restart, and open it again; choose **Allow** when asked.

## Support

Problems or questions: [support@blinken-labs.com](mailto:support@blinken-labs.com).
