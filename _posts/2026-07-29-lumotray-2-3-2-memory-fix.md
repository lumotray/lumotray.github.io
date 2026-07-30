---
layout: post
title: "LumoTray 2.3.2: Memory Fix and a Better Getting-Started Experience"
date: 2026-07-29 19:30:00 +0000
category: update
---

LumoTray 2.3.2 is now available on the Microsoft Store. This release is a focused stability update that addresses the memory pressure introduced in 2.3.1, plus a few quality-of-life improvements.

## What's fixed

**Memory usage for static images.** The way LumoTray renders static images for wallpapers, screensavers, and the lock screen has been reworked to use less memory. This is especially noticeable with large images and multi-monitor setups, where the previous approach could push memory usage higher than it needed to be. If you noticed extra RAM consumption after updating to 2.3.1, this release should bring things back to normal.

**NASA EPIC credits no longer hidden.** The photo credit and timestamp overlay on NASA EPIC wallpapers was getting tucked behind the Windows taskbar. It now sits above the taskbar where it belongs.

**License reminder timing.** On a fresh install, LumoTray no longer shows the license reminder immediately. The first reminder now waits until you have actually had a chance to use the app.

## What's new

**Refreshed getting-started wizard.** The first-run setup wizard has been redesigned with a guided tour of LumoTray's feature set. If you have been using LumoTray for a while and skipped past the wizard on day one, you can replay it anytime from **Settings &rarr; About**.

## What's improved

**NASA EPIC rotation range.** The rotation interval for NASA EPIC images now goes from 10 seconds all the way up to 23 hours, 59 minutes, and 59 seconds. Previously the maximum was 10 minutes, which was too short if you wanted a single Earth image to linger through the workday.

**Consistent mode ordering.** The wallpaper, screensaver, and lockscreen mode dropdowns now share the same ordering, so finding a mode feels the same across all three sections.

## Get it

The update is live on the Microsoft Store. If you have automatic updates enabled, it should install on its own. Otherwise, <a href="https://get.microsoft.com/installer/download/9nwsvm0n0dvc?CID=blog_post_2_3_2">grab it directly from here</a>.
