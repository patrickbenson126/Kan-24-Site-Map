# Kan 24 site map

Where Kan 24, our Peace Corps Guatemala cohort, will be living for the next two years. One file: `index.html`.

## Using it

- Tap a pin or a name to see someone's site. Prev / Next steps through everyone.
- **Directions**: open a card and choose where you're starting from: your current location, Magdalena, or another volunteer's site. The route is drawn on the map with a rough drive time. **Open in Google Maps** hands off to turn-by-turn directions, where you can switch to transit.
- **Copy link** gives a link straight to that person, for example `…/#liza-siegel`.
- Map styles: Simple (works offline), Roads, Terrain, Satellite.

Drive times come from OpenStreetMap road data and run optimistic on mountain roads. Buses take longer.

## Editing the data

Open `index.html` in a text editor and find `COHORT DATA`. One line per person:

```js
{name:"Liza Siegel", site:"Town", dept:"Department", lat:14.6800, lon:-90.7040},
```

Pins sit on each municipio's town center. To move someone to their actual community, change their `lat` / `lon`.

## Updating the site

Replace `index.html` in the repo (Add file → Upload files) and commit. GitHub Pages updates in about a minute, and the link stays the same.

## Credits

Boundaries: Natural Earth via Highsoft map collection (CC BY-NC). Basemaps: Esri. Routing: OSRM demo server, © OpenStreetMap contributors. Department outlines are simplified, so a town right on a border can sit just across the drawn line.
