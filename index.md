# Tlikes privacy policy

**Developer:** Yoann Flament

**Contact:** flament.yoann.pro@gmail.com

**Effective date:** 24/09/2026

## Summary

Tlikes lets you manually sign in to TikTok Web and build a private library of your Likes on your Android device. The developer does not operate an app backend, does not receive your library, and uses no advertising or analytics SDKs.

## Data handled on the device

The app stores:

- the TikTok Web session, managed by Android WebView;
- for each liked video: its identifier, creator name, description, publication time, duration and relative Like order, plus a small cover image;
- data derived from those videos to search and browse them: a normalized copy of the creator and description, and the hashtags of the description;
- the Favorite, To rewatch and watched marks you set, and the names of the collections you create with the videos you put in them;
- the date a video was refused by TikTok's player, so it is skipped for 30 days;
- import checkpoints and pseudonymous source hashes, so an interrupted refresh can resume;
- preferences;
- bounded technical diagnostics and performance measurements: counts, sizes and durations only, such as the duration of the last ten launches, memory use, scrolling smoothness and the network volume of a refresh.

These data remain in Android private app storage. They are excluded from cloud backup and device transfer.

## Network communication and third parties

When you choose to open TikTok, refresh your Likes or play a video, the embedded WebView communicates directly with TikTok over HTTPS. The built-in player loads the video you chose and its two neighbours from TikTok, so that swiping is immediate. While a refresh runs, the TikTok page does not load its pictures, videos or sounds. The app also downloads each video's cover image directly from TikTok's image servers over HTTPS, without your TikTok cookies. When you leave the TikTok screen, its page is released; your session stays until you sign out.

TikTok may process sign-in details, cookies, device and network information, and page requests under its own privacy policy. The app does not read passwords, fill in sign-in forms, extract cookies, or send stored library data to the developer.

## Sharing and export

The app does not automatically share or sell personal data.

- A library export is created only after you explicitly choose an output file with Android's document picker.
- A library file is restored only after you explicitly choose it with the same picker. It is read on the device and never sent anywhere.
- The diagnostic report can be exported to a file you choose or copied to the clipboard, only after an explicit action. It holds technical states, counts, sizes and durations, not your videos.
- The player's diagnostic can likewise be copied to the clipboard.

Exported files and clipboard contents are then controlled by you and the apps you choose.

## Retention and deletion

Data remain on the device until you delete them. On the app's welcome screen, **Privacy & data** shows what is stored, with its size, and lets you delete it. Each action asks for confirmation first:

- **Sign out of TikTok on this phone** clears the TikTok session, cookies and website data, and keeps your library.
- **Delete the covers** removes the cover images; they are downloaded again at the next full check.
- **Remove the videos no longer in your Likes** removes the videos the last full check no longer found in your Likes, with their marks, their place in collections and their covers.
- **Delete local data** makes Android clear all of the app's private data: the library, import checkpoints, preferences, diagnostics, cache and TikTok Web session.

Uninstalling the app, or using Android's **Clear storage** action, also deletes all of these data.

## Security

The app accepts only explicitly allowed HTTPS origins, cancels TLS errors, blocks cleartext traffic, validates messages crossing WebView boundaries, and keeps WebView debugging disabled in release builds. No security measure can eliminate all risk, and TikTok Web behavior can change independently of the app.

## Children's privacy

The app is not directed to children. It relies on a TikTok account, which is subject to TikTok's own age requirements.

## Changes

Material changes to this policy will be published on this page with a new effective date.
