# Tlikes privacy policy

**Developer:** Yoann Flament

**Contact:** flament.yoann.pro@gmail.com

**Effective date:** 27/09/2026

## Summary

Tlikes builds a private library of your TikTok Likes on your Android device, from the file TikTok gives you when you download your data. Tlikes never signs in to TikTok. The developer does not operate a server, does not receive your library, and uses no advertising or analytics SDKs.

## The file you import

You request your data from TikTok, download the file TikTok prepares, and choose it in Android's document picker. Tlikes reads it on the device, as a stream, and keeps only the list of your Likes: for each one, the video's number and the date you liked it. Your messages, profile, purchases, history and every other part of the file are ignored: they are neither kept, nor shown, nor sent anywhere. Tlikes does not keep a copy of the file.

## Data kept on the device

The app stores:

- for each liked video: its number, the date you liked it, its publication time (which the number carries), and its place in your Like order;
- whether TikTok still shows the video, and when that was checked;
- the date a video was refused by TikTok's player, so it is set aside for 30 days;
- the Favorite, To rewatch and watched marks you set, and the names of the collections you create with the videos you put in them;
- the state of the last import: when it ran, and how many Likes it added or no longer found;
- for a library created by an earlier version of Tlikes, which read Likes from TikTok's website: the creator name, description, duration and small cover image it had saved, and a normalized copy of that text to browse it;
- the cookies and storage of TikTok's player, including your cookie choice for TikTok;
- preferences;
- bounded technical diagnostics and performance measurements: states, counts, sizes and durations only, such as the duration of the last ten launches, memory use, scrolling smoothness and the network volume of the player.

These data remain in Android private app storage. They are excluded from cloud backup and device transfer.

## Network communication and third parties

Tlikes communicates only with TikTok, directly and over HTTPS:

- **Checking which videos still exist.** TikTok's file also lists videos that were since deleted or made private. After an import, Tlikes asks TikTok's public embed service (oEmbed, `https://www.tiktok.com/oembed`) once about each video, sending only the video's number, without cookies. It keeps only whether TikTok still shows the video; the title, creator and picture in TikTok's answer are discarded. A video TikTok no longer shows is hidden from your library. This runs in the background, at most 10 questions per second, and only while the device has a connection.
- **Playing a video.** Videos play in TikTok's official embedded player. It loads the video you chose and its two neighbours from TikTok. The first time, a TikTok page asks for your cookie choice for TikTok; that choice and the player's cookies are kept on the device.
- **Opening a video in TikTok.** The **TikTok** button hands the video's public address to TikTok's app or your browser.

TikTok processes these requests, and may process device and network information, under its own privacy policy. Tlikes does not send your library, your marks or your collections to TikTok or to anyone else.

## Sharing and export

The app does not automatically share or sell personal data.

- A library export is created only after you explicitly choose an output file with Android's document picker.
- A library file is restored only after you explicitly choose it with the same picker. It is read on the device and never sent anywhere.
- The diagnostic report can be exported to a file you choose or copied to the clipboard, only after an explicit action. It holds technical states, counts, sizes and durations, not your videos.
- The player's diagnostic can likewise be copied to the clipboard.

Exported files and clipboard contents are then controlled by you and the apps you choose.

## Retention and deletion

Data remain on the device until you delete them. On the app's welcome screen, **Privacy & data** shows what is stored, with its size, and lets you delete it. Each action asks for confirmation first:

- **Clear TikTok website data** clears the cookies and storage of TikTok's player, and keeps your library. TikTok then asks for your cookie choice again.
- **Delete the covers** removes the cover images an earlier version saved. Tlikes no longer downloads covers.
- **Remove … videos no longer in your Likes** removes the videos your last TikTok file no longer holds, with their marks and their place in collections.
- **Delete local data** makes Android clear all of the app's private data: the library, preferences, diagnostics, cache and TikTok player data.

Uninstalling the app, or using Android's **Clear storage** action, also deletes all of these data. The developer holds none of your data, so there is nothing to delete on the developer's side.

## Permissions

- **Internet** and **network state**: to check which videos still exist and to play them. Android requires the network state permission for background work that needs a connection.

## Security

The app accepts only explicitly allowed HTTPS origins, cancels TLS errors, blocks cleartext traffic, validates messages crossing WebView boundaries, and keeps WebView debugging disabled in release builds. It reads TikTok's file with size limits and treats its content as untrusted. No security measure can eliminate all risk.

## Children's privacy

The app is not directed to children. It works with data from a TikTok account, which is subject to TikTok's own age requirements.

## Changes

Material changes to this policy will be published on this page with a new effective date.
