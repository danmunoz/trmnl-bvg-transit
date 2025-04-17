# BVG - Berlin Public Transit (TRMNL)

This is a TRMNL plugin that monitors the status of Berlin's BVG public transportation for a specific stop.

<img width="816" alt="BVG-TRMNL" src="https://github.com/user-attachments/assets/1951bc8e-6698-47bb-8051-c9fb79ec3009" />

---

## Getting Started

### Install via Recipe

This plugin is available as a [recipe](https://usetrmnl.com/recipes/39029/install) and can be installed with a single click. Once installed, any future updates to the plugin will automatically be reflected on your device.

Learn more about TRMNL recipes [here](https://help.usetrmnl.com/en/articles/10122094-plugin-recipes).

### How to Find Your Stop ID

To use this plugin, you’ll need the Stop ID of the location you want to monitor.

You can retrieve this by making a GET request to the [BVG locations endpoint](https://v6.bvg.transport.rest/api.html#get-locations). Run the following command in your terminal:

```bash
curl 'https://v6.bvg.transport.rest/locations?query=alexanderplatz&results=1&linesOfStops=true' -s | jq
```

Replace `alexanderplatz` with the name of the stop you're interested in.

---

## Attributions
Transit data is provided by the [BVG API](https://v6.bvg.transport.rest).
