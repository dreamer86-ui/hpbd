# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-page birthday greeting ("Feliz Cumpleaños") written in Spanish. The entire app lives in `index.html` — a self-contained HTML file with inline CSS, SVG, and JavaScript. No build tools, frameworks, or dependencies.

## Development

Open `index.html` directly in a browser. No server or build step required.

## Architecture

- **CSS animations**: keyframe animations for swaying roses, falling petals, floating entrance, sparkle effects, ribbon wave, and glow pulse — all defined in the `<style>` block.
- **SVG bouquet**: Three white roses with stems, leaves, wrapping paper, and ribbon, built with `<ellipse>`, `<line>`, `<polygon>`, and gradient fills (`petalG`, `centerG`, `leafG`).
- **Falling petals**: Generated dynamically via JS at page load (18 `div.petal` elements appended to `<body>` with randomized position, size, speed, and delay).
- **Message card**: A frosted-glass-style card below the bouquet with the greeting text.
