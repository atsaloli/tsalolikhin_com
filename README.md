# tsalolikhin_com
tsalolikhin.com website

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
