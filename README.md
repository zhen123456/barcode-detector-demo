# Return Receiving Barcode Demo

A browser-only return receiving workflow demo:

1. Scan a return order barcode or QR code.
2. Capture an outer package photo.
3. Confirm returned item quantities.
4. Capture an inside-package item photo.
5. Complete the return and continue with the next order.

## Usage

Open `index.html` from a secure context:

- `http://localhost/...`
- `https://...`

Camera access is usually blocked from plain `file://` pages.

## Test Orders

The demo includes mock order data for:

- `RMA-2026-001`
- `RMA-2026-002`
- `RET-10003`

If native barcode scanning is unavailable, use the manual order input to simulate a scan.

## Browser Notes

This demo uses the native browser `BarcodeDetector` API for scanning. If the current browser does not expose `window.BarcodeDetector`, the page will show an unsupported message and the manual input can still be used for workflow testing.

Typical support is strongest on Android Chrome, ChromeOS, and some macOS Chrome versions. Windows Chrome may not support native barcode detection.
