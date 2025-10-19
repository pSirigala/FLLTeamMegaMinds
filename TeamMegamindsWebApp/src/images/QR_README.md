# QR Code Setup

The QR code on the index page provides quick mobile access to the Team Megaminds website.

## Features:
- **Dynamic QR Code**: Generated via QR Server API
- **Mobile-Friendly**: Links to GitHub Pages deployment
- **Interactive**: Click to copy URL to clipboard
- **LEGO-Themed**: Matches site aesthetic with brick shadows and glow effects
- **Toast Notifications**: Visual feedback when URL is copied

## URL Configuration:
Current QR code points to: `https://psirigala.github.io/FLLTeamMegaMinds/TeamMegamindsWebApp/src/docs/`

## Customization:
To update the QR code URL, modify the `data` parameter in both files:
- `src/index.html` (line with QR image)
- `src/docs/index.html` (line with QR image)

## Backup Options:
If the QR API is unavailable, you can:
1. Generate a static QR code image and save it to `/images/`
2. Update the `src` attribute to point to your local image
3. Use alternative QR generation services

## JavaScript Features:
- Click QR code to copy website URL to clipboard
- Animated toast notification confirms successful copy
- Compatible with modern browsers supporting Clipboard API