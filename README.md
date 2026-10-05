# IPS Underwriter Workspace – static web app

## Deploy
Copy this folder to any static HTTP server (IIS, Nginx, Apache, S3, Azure Static Web Apps) and open `index.html`.

Local test:
```
cd export
python -m http.server 8080      # or: npx serve .
```
Then browse to http://localhost:8080/

## What is inside
- `index.html` – the whole app in one file: markup, logic, runtime, Lato font and logo are embedded.

## Charts
Charts load amCharts 5 from the official CDN at runtime:
https://cdn.amcharts.com/lib/5/ (index.js, xy.js, radar.js, map.js, geodata/usaLow.js, themes/Animated.js)
The browser needs access to cdn.amcharts.com. amCharts 5 free use shows a small amCharts logo; a commercial licence removes it.

## Notes
- No build step and no backend; all data is demo data held in the page.
