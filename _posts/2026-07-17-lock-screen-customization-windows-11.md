---
layout: post
title: "How to Customize the Lock Screen in Windows 11 (and Go Further With Multiple Monitors)"
date: 2026-07-17 05:00:00 +0000
category: tips
image: /assets/gfx/screenshots/wp_page_image.png
---

Windows 11 has slowly made the lock screen more customizable. Widgets arrived with the 23H2 update, the June 2026 25H2 cumulative update (KB5095093) cleaned up the default widget experience so new installs start with just Weather instead of four tiles fighting for attention at the bottom of the screen, and you have always been able to set a custom background or slideshow.

But if you run more than one monitor, you hit a wall pretty fast. Windows 11 still treats the lock screen as one image stretched or mirrored across all displays. There is no built-in way to show a different lock screen background on each monitor, and a lot of the wallpaper variety you get on the desktop (Bing Daily, Unsplash, slideshows with separate folders per screen) does not carry over to the lock screen at all.

This post walks through everything Windows 11 actually lets you change on the lock screen, where Microsoft still draws the line, and how to go further with a tool that does not stop at one wallpaper for all screens.

## What Windows 11 gives you out of the box

Open **Settings > Personalization > Lock screen** and you get three options for the background, as Thurrott's [Windows 11 Field Guide](https://www.thurrott.com/books/windows-11-field-guide/personalize-windows-11/337582/customize-the-lock-and-sign-in-screens-2) covers in detail:

**Windows Spotlight.** Microsoft's default. It pulls a new Bing photo every day or two and overlays a caption, a thumbs-up/down button, and occasionally a "Want to see more?" link that opens Edge. The photos are genuinely good. The promotional bits are not. You can reduce them by toggling off "Show the Windows welcome experience" in the same Settings page, but you cannot remove them entirely while keeping Spotlight.

**Picture.** Pick one static image from your PC. JPEG and PNG both work. For a 4K monitor, a 3840x2160 source prevents upscaling softness. If your displays have different aspect ratios (say a 16:9 main screen and a vertical 9:16 side panel), the same image crops differently on each, and you cannot choose a separate image per monitor.

**Slideshow.** Point Windows at a folder and it cycles through the images inside. You can add multiple folders, set the change interval from one minute to one day, and choose whether to shuffle. The slideshow also pauses on battery by default (you can override this in the advanced settings). A few catches, from both the [Thurrott guide](https://www.thurrott.com/books/windows-11-field-guide/personalize-windows-11/337582/customize-the-lock-and-sign-in-screens-2) and user reports on [Microsoft Q&A](https://learn.microsoft.com/en-us/answers/questions/5544055/lock-screen-folder-isnt-supported-because-of-its-l):

- The folder must be on a local drive. Network shares are unreachable when the screen is locked.
- If Windows decides the folder path is unsupported (even when it is local), the slideshow silently falls back to a static image.
- Windows shuffles automatically. You cannot control the order by filename or date.

There is also a toggle for "Get fun facts, tips, tricks, and more on your lock screen." Microsoft calls them tips. Most people call them ads.

## Lock screen widgets: four slots, Microsoft-only

The 23H2 update added a widget strip to the lock screen, and the June 2026 25H2 update [simplified things](https://itstechbased.com/biggest-windows-11-25h2-june-update-in-main-release-faster-apps-new-file-explorer-build-26200-8737-or-kb5095093/) for new installs: Weather appears as the only default instead of four widgets crowding the bottom of the screen. You can add more through Settings > Personalization > Lock screen, up to a maximum of four.

The available widgets as of mid-2026 are Weather, News headlines, Sports scores, Finance tickers, Calendar appointments, and Traffic estimates. These are all Microsoft widgets. Third-party apps like Rainmeter or Themia cannot place their content on the lock screen, as [Themia's own lock screen guide](https://www.themia.app/blog/how-to-customize-windows-11-lock-screen) explicitly notes: "Third-party desktop widget apps do not integrate with the lock screen."

If you have two or more widgets enabled, you can drag them in the list to reorder left to right. You can also click the "..." menu on Weather to switch between Celsius and Fahrenheit or change the location. That is about as deep as the customization goes.

One oddity worth knowing: the "Suggest widgets for your lock screen" toggle does not suggest anything. It adds three specific widgets (Daily Wonder, Daily Discovery, Events Near You) to your lock screen, period. Thurrott calls out the misleading label, and it has been that way for years.

## What is missing, in a single sentence

Windows 11 has no concept of per-monitor lock screen wallpapers.

Every background option (Spotlight, Picture, Slideshow) applies the same image to every connected display. If your monitors have different resolutions, orientations, or aspect ratios, you get crops and stretches that you cannot fix per-screen.

Themia.app's [lock screen customization breakdown](https://www.themia.app/blog/how-to-customize-windows-11-lock-screen) puts this in a "Cannot change without third-party tools" category: per-monitor lock screen images, custom HTML or interactive lock screens, and third-party widget data are all out of reach natively.

The per-monitor gap is not a bug. It is a design limitation that has persisted across multiple Windows 11 feature updates. Microsoft has invested in lock screen widgets and sign-in screen polish, but the assumption remains that the lock screen is one canvas, not one per display.

People have been asking about this. On [Reddit's r/Windows11](https://www.reddit.com/r/Windows11/comments/1n27k5b/how_do_you_modify_windows_11_lockscreen/), users report that Settings pages for lock screen customization freeze or disappear when third-party personalization tools are active. On [r/WindowsHelp](https://www.reddit.com/r/WindowsHelp/comments/1qgcx2e/windows_spotlight_option_missing_from_lock_screen/), the Spotlight option sometimes vanishes from the dropdown for no obvious reason, leaving only Picture and Slideshow. These are not showstoppers, but they suggest the lock screen personalization stack was not built for power users.

## Going further: per-monitor lock screen wallpapers

LumoTray takes the same wallpaper modes you get on the desktop (images, slideshows, Bing Daily, Unsplash, Wallhaven, Astronomy Picture of the Day, solid colors, video playlists) and applies them to the lock screen too. The difference is that LumoTray treats each monitor as its own canvas, so you can set:

- A static image on your main monitor and a slideshow on your second.
- Bing Daily on one screen and Unsplash on another.
- Different slideshow folders with different intervals per display.
- A solid color on one monitor and a video wallpaper on another.

You can also keep your desktop wallpapers and lock screen wallpapers completely separate. Some people prefer a clean, minimal lock screen with a single photo while their desktop rotates through an Unsplash feed. Others want the lock screen to match the desktop exactly so the transition looks intentional. LumoTray supports both.

Windows 11 does not give you per-monitor lock screen control at all. That is the main reason someone with a multi-monitor setup looks for a third-party tool in the first place.

## Setting it up

Once LumoTray is installed, right-click its tray icon and open the main window. The Wallpaper page is where you configure both desktop and lock screen backgrounds.

![LumoTray wallpaper page](/assets/gfx/screenshots/wp_page_image.png)

For each monitor, you pick a wallpaper mode: Image, Slideshow, Bing Daily, Unsplash, Wallhaven, APOD, Solid Color, Video Playlist, and a few others. Below the mode settings, there is a checkbox labeled **Apply to lock screen**. Check it, and LumoTray writes your per-monitor wallpaper configuration to the lock screen.

If you want one monitor on the desktop to show a slideshow while the lock screen uses a static image, set the desktop mode to Slideshow and the lock screen mode to Image with a different source. The settings live independently.

The same applies to Bing Daily and Unsplash sources. You can have your desktop pull a fresh photo every day while the lock screen shows a static wallpaper you chose once and never want to change. Or flip it: lock screen gets the daily surprise, desktop stays consistent.

## Beyond wallpapers: screensavers and hot corners as lock screen tools

LumoTray also includes screensaver modes (Museums artwork, NASA EPIC imagery, Matrix video overlay, clock displays) and hot corners. These are not lock screen features in the strict sense, but they work well alongside lock screen customization.

**Screensavers as a lock screen alternative.** If you set a screensaver to trigger after a few minutes of inactivity and enable "On resume, display logon screen" in Windows' screensaver settings (the old Control Panel dialog, still accessible by searching "screen saver" in Start), you get a visual display that serves the same purpose as a lock screen when you step away from your desk. The difference is you get per-monitor control over what plays on which screen. A Matrix video on the left monitor and a clock on the right, for example.

**Hot corners to trigger lock.** You can assign the Windows lock action (Win+L) to any corner of any monitor through LumoTray's hot corners page. Move your mouse to that corner and the screen locks. The lock screen wallpaper you set appears, per-monitor.

![LumoTray hot corners page](/assets/gfx/screenshots/hotcorners_page.png)

## One limitation to know

LumoTray's lock screen wallpaper handling works by writing your chosen images to the Windows lock screen cache. It respects whatever wallpaper mode you have configured per monitor and updates the cache when wallpapers change. This works reliably with static images and slideshows.

The lock screen cache is still a Windows-managed thing, though. If Windows has the "Show lock screen background picture on the sign-in screen" toggle off, your sign-in screen will show a solid color regardless of what LumoTray sets. Same goes for the blur effect on the sign-in screen: that is a Windows setting, not something LumoTray controls.

Also, Windows Spotlight on the lock screen is Microsoft's own feed. If you want daily fresh wallpapers on the lock screen without the Spotlight ads, LumoTray's Bing Daily or Unsplash modes on the lock screen give you the same concept without the promotional overlays.

## If you only have one monitor

The built-in Windows lock screen options are probably fine. Pick a nice photo for the Picture mode, or point the slideshow at your Pictures folder. You can add a Weather widget and call it done.

The moment a second monitor appears, the single-canvas limitation becomes obvious. That is when a tool that understands per-monitor lock screen wallpapers stops being a nice-to-have and starts being the reason you installed it.

---

**Set up per-monitor lock screen wallpapers with LumoTray.**

<a href="https://lumotray.com/download/blog_post_lock_screen_windows_11"
   class="store-button"
   onclick="gtag('event', 'store_download_click', {
     download_cid: 'blog_post_lock_screen_windows_11',
     destination_url: 'https://get.microsoft.com/installer/download/9nwsvm0n0dvc?CID=blog_post_lock_screen_windows_11',
     transport_type: 'beacon'
   })">
  Download LumoTray
</a>

*Also read: [How to Set Different Wallpapers on Multiple Monitors in Windows 11](/tips/how-to-set-different-wallpapers-on-multiple-monitors-windows-11/), [Per-Monitor Wallpaper Slideshow Setup](/tips/per-monitor-wallpaper-slideshow-windows-11/), and [How to Add Hot Corners to Windows 11](/tips/how-to-add-hot-corners-to-windows-11/).*
