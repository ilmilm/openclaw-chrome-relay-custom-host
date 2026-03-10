# OpenClaw Browser Relay (Custom Host)

Chrome extension for attaching OpenClaw to an existing Chrome tab via a CDP relay server — with **configurable host/IP + port**.

## Features
- Configure **Host/IP** and **Port** in Options
- Default: `127.0.0.1:18792`
- Stores Gateway token securely in extension local storage

## Install (Chrome)
1. Download or clone this repo.
2. Open `chrome://extensions`.
3. Enable **Developer mode**.
4. Click **Load unpacked** and select this folder.
5. Click the extension icon on the target tab to attach/detach.

## Configure
Open the extension **Options** page and set:
- **Host / IP**: e.g. `127.0.0.1` (local) or `10.0.0.177` (LAN)
- **Port**: Relay port (Gateway port + 3). Default `18792`
- **Gateway token**: must match `gateway.auth.token`

## Security Notes
- If you use a LAN IP, ensure your relay is properly secured.
- Anyone who can reach the relay + token can control the attached tab.

## License
MIT
