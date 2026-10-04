# Lindiwe Dlomo: XR portfolio

A portfolio site with one featured project: **Digital Skills Lab**, a WebXR learning prototype that runs in a desktop browser, on a phone, in a VR headset, and in AR on supported devices.

**Live site:** `https://lindiwed-collab.github.io/AR-VR-Portfolio/`
**Prototype:** `https://lindiwed-collab.github.io/AR-VR-Portfolio/xr-lab/`

## What Digital Skills Lab is

A short immersive learning experience about everyday digital skills. Learners enter a 3D lab and complete three missions:

| Mission | What the learner does | Skill |
| --- | --- | --- |
| Spot the phish | Reads four emails and decides which are scams, then sees why | Online safety |
| Build a strong password | Taps character tiles while a live meter and five rules respond | Account security |
| Sort the files | Matches six files to Documents, Pictures or Music | File management |

Finishing all three earns the *Digital Skills Starter* badge. It is a prototype of the concept behind my VR and AR learning work at TechBridge Innovations, built in 2026 to show how the interaction and spatial UI work in practice.

## Design notes

- **One input model everywhere:** point and select. Mouse, touch and VR controller rays all use the same clickable panels.
- **Spatial UI:** every panel is drawn to a canvas and placed in 3D, so text stays sharp and legible at arm's length in a headset.
- **Immediate feedback:** each choice explains why it was right or wrong, with a short sound cue (toggle in the HUD).
- **AR mode:** the virtual environment hides so the lab appears in the learner's own room.
- The interaction flow diagram is in `img/xr-lab-flow.png`.

## Run it locally

```bash
python3 -m http.server 8000
# then open http://localhost:8000/
```

Open `/xr-lab/` for the prototype. A web server is recommended over double-clicking the file, and VR/AR sessions require HTTPS (GitHub Pages provides this).

## Publish on GitHub Pages

1. Create a new public repository and upload the contents of this folder (`index.html`, `xr-lab/`, `img/`, `README.md`).
2. Go to **Settings > Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
3. After a minute your site is live at the address shown on that page. Update the links at the top of this file.
4. Open it in a private browser window to confirm it is public.

## Test on a device

- **VR headset (for example Meta Quest):** open the `/xr-lab/` link in the headset browser and press the VR button.
- **Phone:** open the link and tap to interact. Landscape works best.
- **AR:** on an AR-capable Android phone using Chrome, press the AR button.

## Built with

- [A-Frame](https://aframe.io) 1.7.0 (MIT licence), bundled locally as `xr-lab/aframe.min.js` so the prototype has no CDN dependency
- WebXR, JavaScript and HTML Canvas

## Author

Lindiwe Dlomo, Johannesburg, South Africa
[LinkedIn](https://linkedin.com/in/lindiwedlomo-b50050b8) | [GitHub](https://github.com/LindiweD-Collab) | lindiwed@techbridgeinnovations.co.za
