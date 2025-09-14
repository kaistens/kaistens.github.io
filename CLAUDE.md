# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Kaistens is a static single-page website for a German catering business specializing in Spanferkel (suckling pig), Flammlachs (flame-grilled salmon), and BBQ catering services.

## Architecture

- **Single HTML file**: All code is contained in `index.html` (532 lines)
- **No build process**: Pure HTML/CSS/JavaScript - directly served by any web server
- **No dependencies**: No npm packages, frameworks, or external libraries
- **Embedded styles and scripts**: CSS (lines 7-340) and JavaScript (lines 492-530) are inline

## Development Commands

Since this is a static site:
- **Run locally**: Open `index.html` directly in a browser or use any static server:
  - `python -m http.server 8000`
  - `npx serve`
  - `php -S localhost:8000`

## Key Components

- **Navigation**: Fixed header with smooth scrolling (JS at lines 499-512)
- **Mobile menu**: Toggle functionality (JS at lines 494-496)
- **Gallery placeholders**: Dynamic content generation (JS at lines 524-529)
- **Responsive breakpoint**: 768px for mobile view

## Asset Structure

- **images/**: Contains 36 JPEG images and 1 PNG logo
  - Food photos (Gericht 1-11.jpeg)
  - Ingredients (Zutat 1-18.jpeg)
  - Specialties (Flammlachs.jpeg, Grill.jpeg)
  - Owner photo (Kai.jpeg)
  - Logo (Logo.png)