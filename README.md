# Chrome BarcodeDetector Demo

A minimal browser demo for testing Chrome's native `BarcodeDetector` API with the device camera.

## Usage

Open `index.html` from a secure context:

- `http://localhost/...`
- `https://...`

Camera access is usually blocked from plain `file://` pages.

## Browser Notes

This demo intentionally uses the native browser API only. If the current browser does not expose `window.BarcodeDetector`, the page will show an unsupported message.

Typical support is strongest on Android Chrome, ChromeOS, and some macOS Chrome versions. Windows Chrome may not support native barcode detection.

