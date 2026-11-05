# SlideStudio

A free, offline PowerPoint-style slide editor for macOS (Apple Silicon and Intel).

## Download

Go to the **Releases** page of this repo and download the `.dmg` that matches your Mac:

- `SlideStudio-1.0.0-arm64.dmg` – Macs with Apple chips (M1, M2, M3, M4 …)
- `SlideStudio-1.0.0-x64.dmg` – older Intel Macs

Open the `.dmg` and drag **SlideStudio** into **Applications**.

### First launch (the app is not signed by Apple)

macOS will warn you the first time. Do this once:

1. In Applications, **right-click** SlideStudio and choose **Open**, then click **Open** again.
2. If macOS says the app is "damaged", open Terminal and run:

   ```
   xattr -cr /Applications/SlideStudio.app
   ```

   then open the app again.

## Features

Text, shapes, images, themes, speaker notes, present mode, undo/redo, save/open (`.slides.json`), and export to PDF (print → Save as PDF).

## Building it yourself

**On GitHub (no setup):** push a tag such as `v1.0.0`, or open the **Actions** tab, pick **Build macOS app**, and click **Run workflow**. The `.dmg` files appear on the run page under *Artifacts* (and on the Releases page for tags).

**On your Mac:**

```
npm install
npm start          # run the app
npm run build      # build .dmg files into dist/
```

Requires [Node.js](https://nodejs.org) 18 or newer.
