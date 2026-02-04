# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Riyaaz Pad** is a specialized percussion practice tool designed to mimic the tactile response and ergonomic layout of the Tabla (Indian classical drum). The product enables students to practice complex finger patterns (Bols) silently and portably.

## Current State

This project includes a **landing page** for collecting email signups and validating market demand, plus a product concept document.

## Landing Page

### Tech Stack
- Plain HTML + Tailwind CSS (via CDN)
- No build step required
- ConvertKit for email capture
- Vercel for hosting

### Local Development
Open `index.html` directly in a browser - no server required.

### Deployment
1. Push to GitHub
2. Connect repo to Vercel (vercel.com)
3. Auto-deploys on every push to main

### ConvertKit Setup
1. Create account at convertkit.com
2. Create a new form
3. Replace `YOUR_FORM_ID` in `index.html` (appears in form action URLs)

### Analytics Setup
1. **Vercel Analytics**: Uncomment the script tag at the bottom of `index.html` after deploying
2. **Google Search Console**: Add site after deployment for search query insights

### UTM Tracking
The page automatically captures `utm_source`, `utm_medium`, and `utm_campaign` parameters from URLs and passes them to ConvertKit with signups.

Test with: `?utm_source=test&utm_medium=email&utm_campaign=launch`

## Product Technical Requirements

The physical product features three tactile zones:
- **High-Rebound Rim (Chanti)** - harder durometer for sharp strikes
- **Weighted Center (Syahi)** - damped, high-density material mimicking the black spot
- **Compression Base (Bayan)** - softer surface for pitch-bending pressure simulation

## Future Development Notes

When software components are added to this project (e.g., companion app, sensor integration, CAD automation scripts), update this file with:
- Build and test commands
- Architecture overview
- Development workflow
