# MinLibMap

A mobile-friendly tool for [Minuteman Library Network](https://www.minlib.net/) patrons to map book availability and find the nearest branch with a copy on the shelf.

**Live:** [esakkas24.github.io/minlibmap](https://esakkas24.github.io/minlibmap)

---

## The Problem

The Minuteman catalog's "Where Is It?" feature shows which branches hold a book — but as a plain text list. When you're already in a parking lot trying to decide which library to drive to, scrolling through 20 branch names with no map or distance info is frustrating.

## How It Works

1. Search for a book on [catalog.minlib.net](https://catalog.minlib.net)
2. Click **"Where is it?"** on any result
3. Select all text in the popup and copy it
4. Open MinLibMap, paste, and tap **"Find My Book"**
5. The map highlights branches with copies on the shelf, sorted by distance from your current location

## Features

- **Map view** of all ~50 Minuteman branch locations
- **Paste parser** that reads the catalog's "Where Is It?" table format
- **GPS proximity sorting** — nearest on-shelf branch shown first
- **One-tap directions** to any branch via Google Maps
- **No login, no API key, no tracking** — single static HTML file

## Usage

Open `index.html` directly in any browser, or visit the hosted version at [esakkas24.github.io/minlibmap](https://esakkas24.github.io/minlibmap). No installation or server required.

## Library Coverage

All 37 public libraries and 5 academic libraries in the Minuteman Library Network, including branches for multi-location systems (Cambridge, Brookline, Somerville, Framingham).

## Reporting Issues

If a library location appears in the wrong spot, or a branch name from the catalog doesn't get matched, please [open an issue](https://github.com/esakkas24/minlibmap/issues) with the unrecognized branch name.

## Tech Stack

- [Leaflet](https://leafletjs.com/) 1.9.4 for mapping
- [CartoDB Voyager](https://carto.com/basemaps/) tile layer (free, no API key)
- Vanilla JS, no build step, no dependencies beyond the CDN links

## License

MIT
