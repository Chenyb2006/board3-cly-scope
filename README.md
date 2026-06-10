# Board3 CLY Scope

Browser scope for Board3 CLY.

## Use

1. Open the GitHub Pages site in desktop Chrome or Edge.
2. Plug in the Board3 USB-C data port.
3. Click `Connect`.
4. Select the Board3 `/dev/cu.usbmodem*` or `COM*` serial port.
5. Use `Record every` to capture coarse curve points. During recording, click `Mark` to add labeled experiment events, then `Export` to save a curve PNG, CSV, JSON, or a Markdown report.

## Notes

- Chrome or Edge is required. Safari and Firefox do not support Web Serial.
- The browser must ask before connecting to the serial port.
- Data stays on the local computer; the page reads the USB serial device directly.
- `filter 50/60/50+60` uses ADS1220 line-noise rejection and runs at 20SPS.
- The display window can be expanded up to 10 minutes. `Y span` can be expanded up to 1000mV.
- Recording is intentionally coarse. Each exported curve point aggregates a short time bucket and stores mean plus min/max range, not every raw sample.
- Markers are saved with elapsed time and label, and are drawn as vertical lines in the exported curve PNG.
