# RSF Vehicle Radio Manager

Standalone Windows manager for creating and maintaining custom music packs for **RSF Vehicle Radio** in Arma 3.

The Manager is designed so communities can import their own music, organize it into stations, prepare the required in-game audio, and export a ready-to-distribute music pack without manually editing the base radio mod.

> **Current release:** 0.6.0  
> **Platform:** Windows  
> **Python / Arma Tools required:** No

## Download

Use the **Releases** section of this repository to download the latest Windows build:

**[Download the latest release](https://github.com/miloomt/RSF-Vehicle-Radio-Manager/releases/latest)**

The downloadable ZIP contains the Manager executable and its documentation. Music is **not** included.

## What it does

- Import individual audio files, multiple files, or complete folders.
- Drag and drop music into your project.
- Automatically convert imported tracks to the OGG format used by the radio.
- Generate the additional audio used by the external / Speaker Mode system.
- Create and organize custom radio stations.
- Edit song titles, station names, station frequencies, and station order.
- Search and preview tracks from the library.
- Move or remove tracks without rebuilding the entire collection.
- Keep a persistent preparation queue that can be stopped and resumed.
- Skip identical files already imported into the same project.
- Reuse previous conversions when possible.
- Export a standalone music pack for distribution to your community.

## Quick start

1. Download and extract the latest Manager ZIP.
2. Run **RSF Radio Manager.exe**.
3. Select **New** to create a music-pack project.
4. Select or create a station.
5. Drag songs or folders into the Manager, or use the file picker.
6. Wait for preparation to finish.
7. Review your music in **Library** and configure stations in **Stations**.
8. Open **Share Pack** and select **Export Pack**.
9. Distribute only the exported music-pack folder to your players.

For multiplayer, both the server and players should load:

- **RSF Vehicle Radio**
- Your exported music pack

The official RSF music pack is optional.

## Automatic tools

The Manager downloads the external tools it needs only when they are required.

### FFmpeg

On the first local audio import, the Manager downloads the configured FFmpeg build from the Gyan provider. The download is SHA-256 verified.

After the initial download, local audio conversion can work without downloading FFmpeg again.

### Optional YouTube import

The Manager can also import individual YouTube video links.

On first use of this feature, it downloads **yt-dlp** and **Deno** from their official repositories and verifies the configured downloads.

- Up to 50 individual video links can be added at once.
- Full playlists are not automatically imported.
- No account, password, or cookies are required by the Manager.
- Restricted, private, live, or protected videos may not be available.
- YouTube changes may require a newer Manager version.

**Important:** the download feature does not grant permission to use, redistribute, or publish copyrighted recordings. Only use content you own or have permission to use, and follow the applicable platform terms.

## Audio quality and storage

The Manager provides three preparation profiles:

- Recommended
- Smaller size
- Higher quality

Changing the quality profile affects future imports. Existing prepared songs are not automatically recompressed when a project is opened.

Original files are preserved separately from exported music packs.

## Updating the Manager

To update:

1. Close the Manager.
2. Replace the executable and documentation with the files from the new release.
3. Keep your existing **Data** folder.

The Data folder contains your projects, originals, queue information, and downloaded tools.

Do **not** distribute your personal Data folder.

## Steam Workshop music packs

If you publish a music pack created with the Manager on Steam Workshop:

1. Publish the exported music pack.
2. Set **RSF Vehicle Radio** as a required Workshop item.
3. When changing songs, export and publish a new version of your music pack.
4. You do not need to modify the base radio mod.

For servers using signature verification, sign your exported PBO using your own key and distribute your own `.bikey`.

Never request or distribute RSF's private signing key.

## Files in the release

The official Windows package currently includes:

- `RSF Radio Manager.exe`
- `LEEME.txt`
- `LICENCIA_MANAGER.txt`
- `PYTHON_LICENSE.txt`
- `TERCEROS.txt`
- `CHANGELOG.txt`

FFmpeg, yt-dlp, Deno, and music files are not bundled in the Manager ZIP.

## License

RSF Radio Manager © 2026 RSF.

See [LICENSE.txt](LICENSE.txt) for the Manager license and [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt) for third-party software information.

The license for the packaged Python runtime is distributed inside the official release ZIP.

## Related project

**RSF Vehicle Radio — Custom Radio System**  
Arma 3 vehicle radio system used by music packs generated with this Manager.

---

RSF Vehicle Radio Manager is a community-made tool for Arma 3 and is not affiliated with or endorsed by Bohemia Interactive.
