# Kan 24 site map

Site map for Kan 24, our Peace Corps Guatemala cohort. One file: `index.html`.

## Two modes, one file

| Address | What it shows | Who it's for |
|---|---|---|
| `…/` | **Explore**: everyone placed, search, tap a pin or name, Prev/Next through people | Everyone, on phones and laptops |
| `…/?reveal` | **Reveal**: the wheel, pins drop one at a time | The projector on reveal day |
| `…/#liza-siegel` | Opens Explore zoomed to that person | Sending someone "here's where I am" |

The footer link switches between modes too.

## Reveal day

1. Run the reveal from the copy of `index.html` on your laptop: double-click it, add `?reveal` to the address. The **Simple** map works offline (the map library and boundaries are inside the file). **Roads** and **Satellite** need internet; if they can't load, the page switches back to Simple on its own.
2. Afterwards, push the updated `index.html` to GitHub. That push is what makes the sites public. Before it, the site holds only placeholder data.

## Editing the data

Open `index.html` in a text editor and find `COHORT DATA`. One line per person:

```js
{name:"Liza Siegel", site:"Santo Domingo Xenacoj", dept:"Sacatepéquez", lat:14.680, lon:-90.704},
```

Set `SAMPLE_SITES = false` once the real sites are in.

## Publishing on GitHub Pages

1. Create a new public repo (for example `cohort-map`) and upload `index.html` (and this README).
2. Repo **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
3. After a minute the site is live at `https://<your-username>.github.io/cohort-map/`.

Updating later: replace `index.html` in the repo (Add file → Upload files) and commit. Pages redeploys in about a minute.

## Map styles

- **Simple**: built-in department boundaries, works offline.
- **Roads**: OpenStreetMap.
- **Satellite**: Esri World Imagery with place labels.

The page remembers each visitor's last choice.

Boundaries: Natural Earth via Highsoft map collection (CC BY-NC, personal non-commercial use). Department lines are simplified, so a town right on a border can land on the wrong side.
