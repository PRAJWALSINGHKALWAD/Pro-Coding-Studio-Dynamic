# Dynamic Content Reference

This folder contains reference structure for dynamic content management using GitHub as a backend.

## Folder Structure

### `/ads`
- Reference folder for organizing ad images by type
- Use this structure when uploading to your GitHub repo
- Consider using GitHub CDN URLs for serving images

### `/urls`
- Reference folder for organizing dynamic URL configurations
- Store JSON files for different URL categories

## Recommended Image Sizes for Upload

### Interstitial Ads
- **Size**: 1080x1920 (portrait) or 1920x1080 (landscape)
- **Format**: WebP preferred, PNG fallback
- **File Size**: Max ~500KB
- **Use Case**: Full-screen ads between app transitions

### Banner Ads
- **Standard Banner**: 320x50
- **Format**: WebP/PNG
- **File Size**: Max ~100KB
- **Use Case**: Small ads within UI

### Rewarded Ads
- **Size**: 1080x1080 (square) or 1080x1920 (portrait)
- **Format**: WebP/PNG
- **File Size**: Max ~400KB
- **Use Case**: User-initiated ads for rewards

## Best Practices

1. **WebP Format**: Use WebP for best compression/quality ratio
2. **PNG Fallback**: Always provide PNG versions for compatibility
3. **CDN Usage**: Leverage GitHub's CDN for fast image delivery
4. **Naming Convention**: Use descriptive names with dimensions (e.g., `interstitial_1080x1920.webp`)
5. **Compression**: Optimize images before upload to reduce bandwidth

## Example GitHub Repo Structure
```
your-repo/
├── ads/
│   ├── interstitial/
│   │   ├── ad1_1080x1920.webp
│   │   └── ad1_1080x1920.png
│   ├── banner/
│   │   ├── ad1_320x50.webp
│   │   └── ad1_320x50.png
│   └── rewarded/
├── urls/
│   ├── development.json
│   ├── staging.json
│   └── production.json
└── config/
    └── app_config.json
```
