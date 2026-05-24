# Board3 CLY Scope

Browser scope for Board3 CLY.

## Use

1. Open the GitHub Pages site in desktop Chrome or Edge.
2. Plug in the Board3 USB-C data port.
3. Click `Connect`.
4. Select the Board3 `/dev/cu.usbmodem*` or `COM*` serial port.

## Notes

- Chrome or Edge is required. Safari and Firefox do not support Web Serial.
- The browser must ask before connecting to the serial port.
- Data stays on the local computer; the page reads the USB serial device directly.
- `filter 50/60/50+60` uses ADS1220 line-noise rejection and runs at 20SPS.
