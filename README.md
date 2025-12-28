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



## Local Development

### Prerequisites

You need to have Hugo installed on your system. Hugo is a static site generator written in Go.

**Installation:**

- **macOS**: `brew install hugo`
- **Linux**:
  - Debian/Ubuntu: `sudo apt-get install hugo`
  - Fedora/CentOS: `sudo dnf install hugo`
  - Arch: `sudo pacman -S hugo`
- **Windows**: `choco install hugo-extended` or `scoop install hugo-extended`
- **From source**: See [Hugo installation docs](https://gohugo.io/installation/)

Verify installation:
```bash
hugo version
```

### Running the Development Server

1. Clone the repository:
```bash
git clone https://github.com/atsaloli/tsalolikhin_com.git
cd tsalolikhin_com
```

2. Start the Hugo development server:
```bash
hugo server
```

The site will be available at `http://localhost:1313/`. The server will automatically reload when you make changes to content or templates.

For development with drafts visible:
```bash
hugo server -D
```

### Building the Site

To generate the static site for production:

```bash
hugo
```

This creates the site in the `public/` directory, which can be deployed to any web server.

### Useful Commands

- `hugo new content/page-name.md` - Create a new content page
- `hugo server --disableFastRender` - Disable fast render mode for full rebuilds
- `hugo server --bind 0.0.0.0` - Make server accessible on network
- `hugo --minify` - Build with minified output
