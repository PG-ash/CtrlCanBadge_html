# Can-Badge iPhone BLE Probe R12

This is the current **read-only** live-GATT verification page.

## Deployment

Deploy `site/index.html` unchanged to an HTTPS static host accepted by the Web Bluetooth-capable iOS browser/runtime. No server-side code is required.

For GitHub Pages, the `site` directory contents are sufficient.

## Safety

The page intentionally contains no calls to:
- `readValue()`
- `writeValue()`
- `writeValueWithoutResponse()`
- `startNotifications()`
- OTA/DFU APIs

It only connects and requests known services/characteristics, then records their properties.
