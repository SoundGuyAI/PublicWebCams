# PublicWebCams

Map of publicly accessible camera feeds in Tel Aviv and Brussels. Ramat Hasharon: no verified public camera yet (see the Leads panel on the page).

Static Leaflet page: `index.html` reads `cameras.json` (map markers) and `leads.json` (unverified leads, not on the map). Tapping a marker opens an in-page viewer. Where the operator permits framing, the viewer shows the operator's own camera page in place (their player, ads and branding). Where the operator blocks embedding or hotlinking (OpenCCTV pages, Windy webcams), the camera stays a link-out. Brussels tries the official CC0 city stream and falls back to the city page when the browser blocks cross-site playback. No raw streams are copied or hotlinked.

Run locally: `python3 -m http.server`, then open http://localhost:8000

## Sources
- Tel Aviv: BeachCam Israel camera pages (beachcam.co.il) and GoSurf Israel's Gordon Beach page, found through OpenCCTV listing pages and follow-up research. OpenCCTV pages and Windy webcams block framing, so cameras available only there link out.
- Brussels: City of Brussels webcams (opendata.brussels.be dataset `webcams`, CC0 1.0).
- Leads not used: Brussels Mobility traffic cameras (CC0, but the service needs a login), Wallonia SPW Trafiroutes (outside Brussels).

## Credit
Idea inspired by https://github.com/bilawalsidhu/gods-eye-view (MIT). No code copied.
