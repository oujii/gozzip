# Gozzip Blog

A modern Jekyll blog designed for GitHub Pages hosting, covering trending topics, culture, and interesting discussions from around the web.

## Features

- **Modern Design**: Clean, responsive layout with a professional appearance
- **GitHub Pages Compatible**: Uses only GitHub Pages supported plugins and configurations
- **SEO Optimized**: Built-in SEO tags, sitemap, and feed generation
- **Mobile Responsive**: Fully responsive design that works on all devices
- **Fast Loading**: Optimized CSS and minimal JavaScript for quick page loads
- **Easy Content Management**: Simple post creation with consistent front matter

## Getting Started

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler gem

### Local Development

1. Clone this repository
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Start the development server:
   ```bash
   bundle exec jekyll serve
   ```
4. Open your browser to `http://localhost:4000`

### Creating Posts

1. Create a new file in the `_posts` directory
2. Use the naming convention: `YYYY-MM-DD-title.md`
3. Add front matter at the top of your file:

```yaml
---
layout: post
title: "Your Post Title"
date: 2025-07-21
categories: [category1, category2]
tags: [tag1, tag2, tag3]
---
```

4. Write your content in Markdown below the front matter

### Customization

#### Site Configuration

Edit `_config.yml` to customize:
- Site title and description
- Author information
- Social media links
- Navigation menu items

#### Styling

- Main styles are in `assets/css/main.css`
- CSS variables at the top of the file control colors and spacing
- Responsive breakpoints are defined in the media queries

#### Content Pages

- Add new pages to the `_pages` directory
- Update navigation in `_config.yml` to include new pages

## Deployment

### GitHub Pages

1. Push your code to a GitHub repository
2. Go to repository Settings > Pages
3. Select source branch (usually `main` or `gh-pages`)
4. Your site will be available at `https://username.github.io/repository-name`

### Custom Domain

1. Add a `CNAME` file to the root directory with your domain name
2. Configure DNS settings with your domain provider
3. Enable HTTPS in GitHub Pages settings

## File Structure

```
├── _includes/          # Reusable HTML components
├── _layouts/           # Page templates
├── _pages/             # Static pages
├── _posts/             # Blog posts
├── assets/
│   ├── css/           # Stylesheets
│   └── js/            # JavaScript files
├── _config.yml        # Jekyll configuration
├── Gemfile            # Ruby dependencies
└── index.html         # Homepage
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

For questions or issues, please open an issue on GitHub or contact the maintainers.
