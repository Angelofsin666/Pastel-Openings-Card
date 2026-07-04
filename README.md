# Pastel Openings Card

A modern, elegant and fully configurable Lovelace card for Home Assistant.

Part of the **Pastel UI** project.

![Home Assistant](https://img.shields.io/badge/Home%20Assistant-2025+-41BDF5?style=for-the-badge&logo=homeassistant)
![HACS](https://img.shields.io/badge/HACS-Custom-orange?style=for-the-badge)
![License](https://img.shields.io/github/license/Angelofsin666/Pastel-Doors-and-Windows-Card?style=for-the-badge)

---

## Features

- Modern pastel design
- Visual editor
- Configurable title, subtitle and icon
- Custom color palette
- Door and window support
- Automatic open/closed detection
- Animated summary
- Progress bar
- Popup on tap (More Info)
- Fully responsive
- Mobile / Tablet / Desktop optimized
- HACS compatible

---

## Installation

### HACS (recommended)

Add this repository as a **Custom Repository**.

Category:

```
Dashboard
```

Then install the card and reload Home Assistant.

### Manual

Copy

```
pastel-openings-card.js
```

into

```
config/www/
```

and add the resource

```yaml
url: /local/pastel-openings-card.js
type: module
```

---

## Example

```yaml
type: custom:pastel-doors-windows-card
title: Piano Terra
subtitle: Aperture
icon: mdi:home

color: amber

entities:
  - entity: binary_sensor.porta_ingresso
    name: Porta Ingresso

  - entity: binary_sensor.finestra_cucina
    name: Cucina

  - entity: binary_sensor.finestra_camera
    name: Camera
```

---

## Options

| Option | Description |
|---------|-------------|
| title | Card title |
| subtitle | Subtitle |
| icon | Header icon |
| color | Pastel color |
| entities | List of entities |
| show_progress_bar | Show progress bar |

---

## Supported entities

- binary_sensor
- door
- window
- garage door
- contact sensor

Future versions will also support:

- cover
- input_boolean
- sensor
- custom entity profiles

---

## Roadmap

- Drag & Drop editor
- Custom entity icons
- Custom entity names
- Area selection
- Label selection
- Automatic grouping
- Universal Openings Card
- Pastel UI Core integration

---

## Part of Pastel UI

This card is part of the **Pastel UI** collection.

Current projects include:

- Pastel Lights Card
- Pastel Doors & Windows Card
- Pastel Climate Card *(coming soon)*
- Pastel Appliance Card *(planned)*
- Pastel Pool Card *(planned)*
- Pastel Robot Card *(planned)*
- Pastel Energy Card *(planned)*

---

## License

MIT License

---

Made with ❤️ for the Home Assistant community.
# Pastel-Openings-Card
