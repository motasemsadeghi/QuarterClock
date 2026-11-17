# Quarter Clock | ساعت چهارتکه

An analog clock drawn as a quarter circle. Seconds, minutes and hours each sweep their own quarter arc, and the whole face turns 90° as the day moves on.
ساعت آنالوگ روی یک ربع دایره، با سه کمان برای ثانیه، دقیقه و ساعت.

## How it works | طرز کار

- **Three nested quarter arcs** around one pivot in the bottom-left corner: seconds (outer), minutes (middle) and hours (inner).
- **Seconds and minutes:** each arc covers 15 units. The labels change every quarter (for example 0–15, then 15–30, 30–45, 45–60) while the hand sweeps from start to end of the arc.
- **Hours:** the arc covers 6 hours on a 24-hour scale, so the labels move through four quarters a day.
- **The face rotates:** every time the hour hand enters a new quarter of the day, the whole clock turns 90° with an eased animation. Labels are counter-rotated so the numbers always stay upright.
- **Smooth hands:** the hands move continuously (updated every frame), not in jumps.
- **Persian digits** for all numbers, shown with the Vazirmatn font.

## Features | ویژگی‌ها

- Automatic light and dark theme (follows the device setting).
- Responsive: scales to the screen size and respects iPhone safe areas.
- Installable as a web app (PWA) with an offline service worker.
- One HTML file with plain JavaScript and SVG, no libraries.

## Usage | نحوهٔ استفاده

Open `index.html` in a modern browser, or host the folder on GitHub Pages and add it to the home screen.

For the install and offline features, keep these files next to `index.html`:

```
index.html
manifest.webmanifest
sw.js
icon-192.png
```

The Vazirmatn font loads from Google Fonts. Without a connection it falls back to Tahoma or the system font.

## Author

Motasem Sadeghi

## License

[MIT](LICENSE)
