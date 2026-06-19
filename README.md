# Social Media Images Repository

Public image hosting for PostStream social media posts across multiple brands and content types.

## Repository Structure

```
social-media-images/
├── command-openclaw/          # Main AI/tech brand
│   ├── posts/                 # Feed posts (Instagram, Facebook, etc.)
│   ├── stories/               # Stories content
│   └── reels/                 # Short-form video thumbnails
│
├── mountainside-scoop/        # Local newsletter
│   └── newsletter/            # Newsletter header images, graphics
│
├── profit-hub/                # Affiliate marketing & hosting
│   ├── affiliate/             # Affiliate product promotions
│   └── hosting/               # Web hosting service promos
│
├── local-business/            # Local business network
│   ├── mountainside/          # Mountainside, NJ specific
│   └── general/               # General local business content
│
└── [future-brands]/           # Add new brands as needed
```

## URL Pattern

All images are accessible via raw GitHub URLs:

```
https://raw.githubusercontent.com/TBrend/social-media-images/main/{brand}/{type}/{filename}
```

### Examples:

- **Command OpenClaw posts:**
  - `https://raw.githubusercontent.com/TBrend/social-media-images/main/command-openclaw/posts/2026-06-19-morning.png`

- **Mountainside Scoop newsletter:**
  - `https://raw.githubusercontent.com/TBrend/social-media-images/main/mountainside-scoop/newsletter/june-header.jpg`

- **Profit Hub affiliate:**
  - `https://raw.githubusercontent.com/TBrend/social-media-images/main/profit-hub/affiliate/product-launch.png`

- **Local business:**
  - `https://raw.githubusercontent.com/TBrend/social-media-images/main/local-business/mountainside/restaurant-spotlight.jpg`

## Naming Convention

**Format:** `YYYY-MM-DD-{descriptor}.{ext}`

**Examples:**
- `2026-06-19-morning.png` - Morning post for June 19
- `2026-06-19-midday.jpg` - Midday post for June 19
- `2026-06-19-evening.png` - Evening post for June 19
- `june-newsletter-header.jpg` - Newsletter header
- `summer-sale-promo.png` - Promotional graphic

## Supported Formats

- **PNG** - Best for graphics with transparency
- **JPG/JPEG** - Best for photos (smaller file size)
- **GIF** - For animated content (stories/reels)
- **WebP** - Modern format (check platform support)

## Platform Requirements

| Platform | Max Size | Recommended Size | Format |
|----------|----------|------------------|--------|
| Instagram | 8 MB | 1080x1080 | JPG/PNG |
| Facebook | 8 MB | 1200x630 | JPG/PNG |
| Bluesky | 1 MB | 1200x1200 | JPG/PNG |
| LinkedIn | 8 MB | 1200x627 | JPG/PNG |
| Twitter/X | 5 MB | 1200x675 | JPG/PNG |

## Adding New Brands

To add a new brand or content type:

1. Create the folder structure: `new-brand/content-type/`
2. Update the upload script to support the new path
3. Document the new brand in this README
4. Update TOOLS.md in the workspace

## Automation

Use the upload script in the workspace:
```bash
~/.openclaw/workspace-social-media-guy/scripts/upload-image-to-github.sh
```

See TOOLS.md for detailed usage instructions.
