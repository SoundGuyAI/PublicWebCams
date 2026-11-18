# PublicWebCams

Map of publicly accessible camera feeds in Tel Aviv and Brussels. Ramat Hasharon: no verified public camera yet (see the Leads panel on the page).

Static Leaflet page: `index.html` reads `cameras.json` (map markers) and `leads.json` (unverified leads, not on the map). Every camera is a link-out to the operator's own page; nothing is embedded or copied.

Run locally: `python3 -m http.server`, then open http://localhost:8000

## Sources
- Tel Aviv: BeachCam Israel cameras, found through OpenCCTV listing pages. OpenCCTV blocks framing.
- Brussels: City of Brussels webcams (opendata.brussels.be dataset `webcams`, CC0 1.0).
- Leads not used: Brussels Mobility traffic cameras (CC0, but the service needs a login), Wallonia SPW Trafiroutes (outside Brussels).

## Credit
Idea inspired by https://github.com/bilawalsidhu/gods-eye-view (MIT). No code copied.
