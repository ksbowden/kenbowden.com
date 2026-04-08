# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal splash page for kenbowden.com. The entire site is a single `index.html` file — no build step, no bundler, no dependencies beyond Google Fonts (Space Grotesk).

## Development

Open `index.html` directly in a browser. No server required, though any static file server works (e.g., `python3 -m http.server`).

## Architecture

Everything lives in `index.html`: markup, CSS (`<style>` block), and JavaScript (`<script>` block at the end of `<body>`).

### Design Theme

The site uses a **CRT TV / retro monitor** aesthetic. Key effects:

- **Chromatic aberration** on the heading text (animated pink/cyan text-shadow shifts)
- **Custom cursor** with chromatic aberration (pink and cyan offset circles tracking the mouse)
- **Mouse-follow brightness glow** simulating CRT phosphor response
- **Click ripple** effect (pink/cyan expanding circles, like tapping a CRT screen)
- **Scanlines**, a sweeping **scan bar**, subtle **screen flicker**, and **vignette** overlays
- **Ambient glow** with a breathing animation

### Color Palette

- Background: `#131313`
- Text: `#e5e2e1`
- Pink/magenta accent: `rgba(255, 171, 243, ...)`
- Cyan accent: `rgba(0, 221, 221, ...)`
- Yellow (footer): `#cdcd00`
- Nav icons: `#00dddd`

When adding new elements or effects, maintain consistency with this CRT theme and color palette.
