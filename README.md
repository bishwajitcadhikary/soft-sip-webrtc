<h1 align="center">
  <br>
  Soft SIP WebRTC Client
  <br>
</h1>

<h4 align="center">A sleek, modern, browser-based softphone built with SIP.js.</h4>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#technologies">Technologies</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#configuration">Configuration</a> •
  <a href="#credits">Credits</a>
</p>

## Overview

**Soft SIP** is a fully functional web-based VoIP softphone. It allows you to connect directly to any SIP/WebSocket compatible PBX server without needing to install standard client applications or browser extensions.

With an aesthetic and responsive dark-mode UI built using Tailwind CSS, it offers an intuitive and modern calling experience right from your browser.

## Features

* **Real-time WebRTC Calling**: Make and receive crisp audio VoIP calls natively in the browser.
* **Modern Interface**: A clean, glowing dark theme built with Tailwind CSS.
* **Session Persistence**: Securely saves your SIP credentials and PBX server configurations across sessions using `localStorage`.
* **Interactive Dialpad**: Complete dialpad with mouse-click and keyboard DTMF tone support while in an active call.
* **Long-press Detection**: Simulates mobile experiences by offering a long-press on `0` to input `+`.
* **Call History Logs**: Automatically logs up to 50 of your Outbound, Inbound, Missed, and Declined calls, with formatted call durations.
* **Interactive Modals**: Seamless settings configurations and incoming call notifications via floating UI modals.

## Technologies

* **HTML5 / Vanilla JavaScript**: Core logic and structural markup. No heavy frameworks!
* [**SIP.js**](https://sipjs.com/): An unopinionated VoIP SIP stack providing WebRTC and WebSocket abstraction.
* [**Tailwind CSS**](https://tailwindcss.com/): Rapid styling framework served via CDN for simple deployment.

## How To Use

Because it doesn't require a build step, getting started is almost instantaneous.

1. Clone this repository or download the ZIP:
```bash
git clone https://github.com/bishwajitcadhikary/soft-sip-webrtc.git
```
2. Navigate into the folder:
```bash
cd soft-sip-webrtc
```
3. Open the `index.html` file in your preferred modern web browser (Chrome, Firefox, Safari, Edge).

*Note: For WebRTC media (microphone access) to work outside of `localhost`, your webpage MUST be served securely over HTTPS.*

## Configuration

When launching the softphone for the first time, click the **Settings Gear Icon** in the top right.

You must provide your PBX provider details:
- **WSS URL:** Your PBX secure WebSocket path (e.g., `wss://you-pbx-ip:7443`)
- **SIP Domain:** Your PBX domain or IP address (e.g., `124pbx.softcents.com`)
- **Extension:** Your SIP account username (e.g., `1001`)
- **Password:** Your SIP account secret

Click **Save Settings** and the client will automatically attempt to register.

## Credits

Developed by [Frolax](https://frolax.agency)
