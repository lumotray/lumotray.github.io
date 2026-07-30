---
layout: post
title: "Windows 11 Finally Lets You Move the Taskbar - But Wallpapers Are Still Stuck in 2021"
date: 2026-07-27 04:30:00 +0000
categories: tips
---

In 2021, Windows 11 shipped without the ability to move the taskbar. You could drag it to the top, left, or right in every version of Windows since 95. Suddenly, you could not. The taskbar was locked to the bottom, and the internet spent four years complaining about it.

That is about to change. Windows 11 build 26300.8493, now in the Insider Experimental channel, finally adds taskbar repositioning back. You can put it on the top, left, or right edge of the screen again. There is also a new compact taskbar mode for smaller screens.

For anyone running a multi-monitor setup, this is genuinely useful. Taskbar at the bottom of a 32-inch 4K display feels fine, but at the top of a vertical side monitor it can be a better fit. The flexibility has been missing since Windows 10.

But here is what did not change: anything related to wallpaper, screensavers, hot corners, or per-monitor personalization. Not in this build. Not in the July 2026 Patch Tuesday update that shipped 570 CVE fixes. Not anywhere on Microsoft's public roadmap for 26H2, which is expected to land this fall.

The taskbar is moving again. The rest of personalization is frozen in 2021.

## What 26H2 actually ships for the taskbar

The taskbar changes are confirmed in build 26300.8493, which Pureinfotech and Windows Central have covered in detail. You can now go to Settings > Personalization > Taskbar > Taskbar behaviors and choose between Top, Bottom, Left, and Right positions. Flyouts, tooltips, and animations follow the taskbar regardless of where you place it. The "Never combine taskbar buttons" option and smaller taskbar icons work across all layouts.

There is also a new compact taskbar size option. Instead of the single auto-scaling mode, you can explicitly choose Small or Default. Small mode reduces height and icon size while keeping Start, Search, and system tray correctly aligned. Useful on laptops with limited vertical space.

These are good changes. They fix a regression that should never have shipped in the first place. But that is also the point: Microsoft is catching up to Windows 10.

## What still has not changed since 2021

While the taskbar gets its overdue fix, here is everything else that multi-monitor users have been waiting for:

**No per-monitor wallpaper support.** Windows 11 can set one wallpaper across all monitors via the Personalization settings. That is it. If you want a different image on each screen, you are doing registry edits or using a third-party tool. There is no timeline for Microsoft to add this.

**No built-in hot corners.** macOS has had hot corners since 2007. Windows has never shipped them. You can approximate one corner action (Quick Settings or Notification Center) through the taskbar settings, but you cannot assign custom actions to each corner. And you definitely cannot run different corner actions per monitor.

**No useful screensavers.** The Windows screensaver panel (still buried in the old Control Panel) offers six screensavers: 3D Text, Blank, Bubbles, Mystify, Photos, and Ribbons. Those have not changed since Windows XP. There is no per-monitor control, no clock mode, no photo browser mode, no useful dashboard.

**No per-monitor wallpaper slideshows.** Windows 11 has a slideshow mode, but it pulls from one folder at one interval for all monitors. You cannot set independent folders or timers per screen. The built-in slideshow has also been buggy. Users on BleepingComputer and the Microsoft forums have reported black screens after sleep/wake since early 2025.

**Screensavers are still one-size-fits-all.** Windows activates the same screensaver across all connected monitors. You cannot run a clock on one screen and photos on another. Microsoft Q&A thread 5846366, from April 2026, confirms this is by design and not changing.

**Virtual desktop wallpaper resets are still happening.** The July Patch Tuesday update (KB5101650) was supposed to address this, but Windows Central reported on July 18 that the fix is incomplete. Some users still see wallpapers revert when [switching desktops](/tips/windows-11-virtual-desktop-wallpaper-reset/). Earlier coverage from PCWorld (July 17) and BleepingComputer (July 15) did not mention any personalization-related fixes in the 570-patch update at all.

**No lock screen wallpaper flexibility.** Windows 11 can set a single lock screen image or a Windows Spotlight slideshow. No custom sources. No per-monitor options. No integration with external wallpaper sources.

Microsoft's 26H2 page, published by Windows Central on July 19, highlights AI-driven security, Smart Answers, improved Search, Point-in-Time Restore, and Screen Tint. The word "wallpaper" does not appear.

## Enter LumoTray: what Microsoft is not building

If you run multiple monitors on Windows 11, you have probably already accepted that native personalization is not enough. Here is what LumoTray does for each of the gaps above. And yes, these are all real, shipping features, not wishlist items.

**Per-monitor wallpaper management.** [LumoTray lets you set a different image, color, slideshow, or live source per monitor](/tips/how-to-set-different-wallpapers-on-multiple-monitors-windows-11/). Solid colors, color faders, local image folders, Unsplash, Wallhaven, Bing daily images, Windows Spotlight, NASA APOD, web pages, PDFs, and live video wallpapers. All assignable independently to each display. Per-monitor fit modes (fill, fit, stretch, tile, center, span) give you fine control over how each wallpaper lands on each screen.

**Hot corners.** [LumoTray can run actions when you move your mouse to any corner of any monitor](/tips/how-to-add-hot-corners-to-windows-11/). You can assign different actions per corner and per display. If you came from macOS and miss the feature, or just want a faster way to launch apps, trigger a screensaver, or lock the screen, this covers it.

**Screensavers that do something useful.** [LumoTray includes a full-screen clock, timer, stopwatch, museum artwork viewer, NASA Earth imagery, Matrix-style video overlay, and Shadertoy support](/tips/bring-back-useful-screensavers-windows-11/), among other modes. You can set a global hotkey to start a specific screensaver, and you can configure screensavers per monitor. Monitor 1 can show a clock while monitor 2 cycles through NASA planet photos.

**Per-monitor wallpaper slideshows.** [Each monitor gets its own folder, its own interval, and its own shuffle setting](/tips/per-monitor-wallpaper-slideshow-windows-11/). Or skip local folders entirely and assign Unsplash to one monitor and Wallhaven to the other, with different refresh rates.

**Lock screen manager.** LumoTray applies the same wallpaper modes to your Windows lock screen (images, slideshows, live sources, NASA APOD) from a dedicated settings section. It does not add per-monitor lock screen wallpaper because Windows itself has no concept of that. (Nobody's app can do what the OS does not support.)

If you have been dealing with Windows 11 wallpaper limitations, LumoTray is available from the Microsoft Store.

<a href="https://get.microsoft.com/installer/download/9nwsvm0n0dvc?CID=blog_post_taskbar_26h2_wallpapers"
   class="download-button">
  Download LumoTray from the Microsoft Store
</a>

---

*Sources: Windows Central (July 19, 2026 - 26H2 overview), Pureinfotech (build 26300.8493 coverage), PCWorld (July 17 - 5 features from July update), BleepingComputer (July 15 - Dell shutdown bug in KB5101650), Microsoft Q&A thread 5846366 (April 2026 - per-monitor screensaver confirmation).*
