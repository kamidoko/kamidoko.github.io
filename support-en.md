---
layout: default
title: Paper Map GPS — Support
description: Support and FAQ for Paper Map GPS (紙どこ), the iOS app that overlays your live GPS location on paper maps.
---

<div class="hero-card" markdown="1">

# Paper Map GPS — Support

Thank you for using Paper Map GPS (Japanese name: 紙どこ).
This page covers frequently asked questions and how to contact us.

[日本語版はこちら / Japanese version](/support.html)

</div>

<nav class="toc-nav" markdown="1">

**Contents**

- [Contact](#contact)
- [Importing maps](#import)
- [Alignment](#calibration)
- [Sharing & purchases](#sharing)
- [Your data](#data)
- [Troubleshooting](#trouble)
- [Links](#links)

</nav>

---

## <span id="contact">📨 Contact</span>

<div class="contact-card" markdown="1">

For questions, bug reports, or feature requests, feel free to reach out:

**📧 Email**　[kamidoko@biz.nifty.jp](mailto:kamidoko@biz.nifty.jp?subject=Paper%20Map%20GPS%20Support)

To help us respond quickly, please include the following if you can:

- Your iPhone model (e.g., iPhone 15 Pro)
- iOS version (e.g., iOS 18.4)
- App version (see Settings → App Info)
- What happened, or what you'd like to ask
- Steps to reproduce (for bugs)
- Screenshots (very helpful)

We usually reply within **3–5 business days**. Support is available in English and Japanese.

</div>

---

## <span id="import">🗺 Importing maps</span>

### Q. What kinds of maps can I import?
A. You can import from the iPhone camera, your photo library, or the Files app (PDF / images). **However, not every map works well.**

✅ **Maps that work**

- **Outdoor maps** (places where GPS works)
- **Maps with a reasonably consistent scale and little distortion**
- Examples: theme-park guide maps, sightseeing maps, hiking trail maps, outdoor festival maps, maps of large parks and botanical gardens

❌ **Maps that are hard to support**

- **Indoor floor plans** (GPS does not work indoors, so your location won't appear)
  - Hospital / airport / shopping-mall floor maps, station concourse maps, exhibition floor plans, etc.
- **Maps with a wildly inconsistent scale** (different scale in different areas)
  - Hand-drawn maps with arbitrary distances, extremely stylized or cartoon-style maps
- **Diagrams that aren't maps**
  - Subway-style diagrams that show connections rather than physical space

An outdoor map with a managed scale and little distortion — that's where this app shines.

### Q. A PDF won't import
A. Password-protected PDFs, PDFs without images (text-only), or PDFs with unusual encryption may fail to load. Taking a screenshot and importing it as an image is the most reliable workaround.

### Q. My imported map looks blurry
A. Accuracy improves when you photograph the map **straight from above**, in good light, **without wrinkles or glare**. For PDFs, quality depends on the original resolution.

---

## <span id="calibration">📍 Alignment</span>

### Q. My current location doesn't appear on the map
A. You need **3 or more** alignment points. Tap at least 3 recognizable landmarks on the map (entrances, corners, intersections, distinctive buildings) and match each one to where you're actually standing.

### Q. My location appears in the wrong place
A. There are **3 main causes**. The most common is that the imported map itself is distorted.

**1. The imported map is distorted (most common)**

If the paper map was captured in a distorted state, an accurate location display is fundamentally impossible. Check whether any of these apply:

- The paper had wrinkles or folds when photographed
- It was photographed **at an angle** (perspective turns rectangles into trapezoids)
- The paper was curved (e.g., held in your hand)
- The original map is **hand-drawn** or **stylized**, with an inconsistent scale

👉 **Fix**: flatten the paper on a desk and re-photograph it **straight from above**. Adding **5 or more** alignment points enables TPS (thin-plate spline), a flexible correction that absorbs local distortion — but extreme distortion cannot be fully fixed.

**2. Alignment point placement**

If your alignment points are **too close together** or **in a straight line**, the map-wide mapping can't be computed well.

👉 **Fix**: place 3 or more points far apart from each other, including near the corners of the map.

**3. GPS signal conditions**

Indoors, in valleys, or between tall buildings, GPS itself becomes inaccurate.

👉 **Fix**: redo the registration outdoors with a clear view of the sky. The translucent blue circle around your location dot shows the **margin of error**.

### Q. I want to redo the alignment
A. Tap "Alignment" at the bottom of the map screen → "Points", then swipe left on a point to delete it individually.

### Q. It says my location can't be calculated
A. Your registered points may be in a straight line or clustered in one place. Add points farther apart from Alignment.

---

## <span id="sharing">👥 Sharing & purchases</span>

### Q. What is a Share Pass?
A. It lets you share a map and live locations with family and friends via iCloud. Only the person who starts the share pays — invited members join **for free** (owner-pays model).

### Q. What passes are available?

| Pass | Price | Details |
|---|---|---|
| **Free 30 Minutes** | Free (one time) | Try sharing free for 30 minutes |
| **24-Hour Share Pass** | ¥300 (one-time) | Valid for 24 hours. Great for a single outing |
| **Monthly Outing Pass** | ¥600 / month (auto-renewing) | For people who share regularly |

Prices are shown in your local currency on the App Store.

### Q. How do I cancel the monthly pass?
A. Any of the following works:

1. iPhone Settings → your Apple ID (at the top) → "Subscriptions"
2. App Store → "Account" → "Manage Subscriptions"
3. In the app: Settings → "Share Pass" → "Manage or Cancel Monthly Pass"

After cancelling, you keep access until the end of the current period.

### Q. I can't see the other person's location
A. Ask them to check the following:

- "Share your location on a shared map" is ON in the app
- Location permission is **"While Using the App" or better**
- **Either** of the following is true:
  - **They have the shared map open** (if you're both looking at the app, this alone is enough)
  - Or "**Share in Background**" is ON and location permission is set to "**Always**" (for sending updates while the screen is off)
- They have a network connection (no updates while offline)

In other words, while **both of you have the shared map open**, no background setting or "Always" permission is needed. Background sharing is only required if you want updates to continue while doing other things.

### Q. How do I stop sharing?
A. Open the shared map and use the "Share" button at the bottom of the screen to stop or leave.

---

## <span id="data">💾 Your data</span>

### Q. Where is my data stored?
A. Map images, alignment points, and markers are stored on your device. Data related to shared maps is also stored in iCloud (CloudKit). See the [Privacy Policy]({{ site.baseurl }}/privacy-en.html) for details.

### Q. Can I transfer data to a new phone?
A. Shared maps sync automatically via iCloud when you sign in with the same Apple ID. Non-shared maps don't transfer automatically, but you can export them as `.gpsmap` files and import them on the new device.

### Q. Is my data deleted when I delete the app?
A. Yes. All data on the device is removed. Shared maps remain in iCloud, so you can re-accept them with the same Apple ID after reinstalling.

---

## <span id="trouble">🔧 Troubleshooting</span>

### Q. I accidentally denied location permission
A. Open iPhone Settings → "Privacy & Security" → "Location Services" → "Paper GPS" and choose "While Using the App" or "Always". You can also jump there directly from the "Open Settings" link on the in-app permission banner.

### Q. The app crashes or feels slow
A. Please try:

1. Fully quitting and relaunching the app
2. Restarting your iPhone
3. Checking free storage in Settings → General → iPhone Storage
4. Making sure the app and iOS are up to date

If it still doesn't improve, contact us with the steps to reproduce and your iOS / app versions.

### Q. The compass points the wrong way
A. The iPhone compass is sensitive to nearby magnetic interference. Moving the iPhone in a figure-eight pattern in an open outdoor area often recalibrates it.

---

## <span id="links">🔗 Links</span>

- [Privacy Policy]({{ site.baseurl }}/privacy-en.html)
- [App Store page](https://apps.apple.com/app/id6779239045)

---

<div class="footer-meta" markdown="1">

Last updated: 2026-07-11

</div>
