# tsalolikhin_com
tsalolikhin.com website

## Photo Gallery

The photography section uses Hugo's built-in image processing to create a professional photo gallery with automatic thumbnails.

### How to Add Photos

1. Place your image files (JPEG, PNG, etc.) in the `content/photography/` directory
2. Hugo will automatically:
   - Generate thumbnails (400x300px)
   - Create optimized full-size versions (1200x1200px max)
   - Display them in a responsive grid layout
   - Enable lazy loading for better performance

That's it! The gallery shortcode will automatically pick up all images in the photography page bundle.

### Example

```bash
# Add a new photo to the gallery
cp my-photo.jpg content/photography/

# Build and view the site
hugo server
```

### Gallery Features

- **Responsive Grid**: Automatically adjusts to screen size
- **Hover Effects**: Images scale slightly and lift on hover
- **Click to View**: Full-size images open in a new tab
- **Optimized**: Automatic image compression and thumbnail generation
- **Fast Loading**: Lazy loading ensures smooth page performance
