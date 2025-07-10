# NiceRestaurant Jekyll Website

This is a Jekyll-powered static website based on the NiceRestaurant Bootstrap template, converted for easy deployment and maintenance.

## Features

- **Responsive Design**: Bootstrap-based responsive layout
- **Modern Jekyll Architecture**: Clean separation of layouts, includes, and content
- **SEO Optimized**: Built-in SEO tags and sitemap generation
- **Easy Customization**: Configurable through `_config.yml`
- **Multiple Sections**: 
  - Hero/Landing section
  - About section
  - Menu showcase
  - Chef profiles
  - Testimonials
  - Event booking
  - Location/Contact information

## Quick Start

### Prerequisites

- Ruby (version 3.0+)
- Bundler
- Jekyll

### Installation

1. Clone or download this repository
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Build the site:
   ```bash
   bundle exec jekyll build
   ```
4. Serve locally:
   ```bash
   bundle exec jekyll serve
   ```
5. Visit `http://localhost:4000` to view the site

## Configuration

### Site Settings

Edit `_config.yml` to customize:

- Site title, description, and contact information
- Restaurant details (name, address, phone, hours)
- Social media links
- SEO settings

### Content Management

#### Restaurant Information
Update restaurant details in `_config.yml`:

```yaml
restaurant:
  name: "Your Restaurant Name"
  tagline: "Your Tagline"
  phone: "Your Phone Number"
  email: "your@email.com"
  address: "Your Address"
  hours:
    weekdays: "Monday - Friday: 11:00 AM - 11:00 PM"
    weekends: "Saturday - Sunday: 10:00 AM - 12:00 AM"
  social:
    facebook: "https://facebook.com/yourrestaurant"
    instagram: "https://instagram.com/yourrestaurant"
    twitter: "https://twitter.com/yourrestaurant"
    youtube: "https://youtube.com/yourrestaurant"
```

#### Menu Items
Menu items are coded directly in `_includes/sections/menu.html`. To add new items, follow the existing HTML structure.

#### Images
Replace images in the `assets/img/` directory with your own:
- `assets/img/restaurant/` - Food and restaurant photos
- `assets/img/person/` - Staff and customer photos
- `assets/img/favicon.png` - Site favicon
- `assets/img/apple-touch-icon.png` - iOS app icon

## File Structure

```
├── _config.yml                 # Site configuration
├── _layouts/
│   └── default.html           # Main layout template
├── _includes/
│   ├── header.html            # Site header
│   ├── footer.html            # Site footer
│   └── sections/              # Page sections
│       ├── menu.html
│       ├── chefs.html
│       ├── testimonials.html
│       ├── book-a-table.html
│       ├── location.html
│       ├── events.html
│       └── contact.html
├── assets/                    # Static assets
│   ├── css/
│   ├── js/
│   ├── img/
│   └── vendor/
├── index.md                   # Homepage content
├── Gemfile                    # Ruby dependencies
└── README.md                  # This file
```

## Customization

### Styling
- CSS files are in `assets/css/`
- Vendor CSS (Bootstrap, etc.) in `assets/vendor/`
- Main styles in `assets/css/main.css`

### Adding New Sections
1. Create a new file in `_includes/sections/`
2. Add the include to `index.md`
3. Style as needed

### Adding New Pages
1. Create a new `.md` file with appropriate front matter
2. Use the `default` layout
3. Add navigation links as needed

## Deployment

### GitHub Pages
1. Push to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Site will be available at `https://username.github.io/repository-name`

### Netlify
1. Connect your repository to Netlify
2. Set build command: `bundle exec jekyll build`
3. Set publish directory: `_site`

### Manual Deployment
1. Run `bundle exec jekyll build`
2. Upload contents of `_site/` directory to web server

## Development

### Local Development
```bash
# Install dependencies
bundle install

# Serve with live reload
bundle exec jekyll serve --watch --host 0.0.0.0

# Build for production
bundle exec jekyll build
```

### Making Changes
- Edit content in `.md` files
- Modify layouts in `_layouts/`
- Update includes in `_includes/`
- Add new assets to `assets/`

## Support

For issues related to the original template, visit: https://bootstrapmade.com/nice-restaurant-bootstrap-template/

## License

This Jekyll conversion maintains the original template's license. Please refer to the BootstrapMade license for details.

## Credits

- Original Template: [NiceRestaurant by BootstrapMade](https://bootstrapmade.com/)
- Jekyll Integration: Custom implementation
- Bootstrap Framework
- Various vendor libraries (see `assets/vendor/` directory)

