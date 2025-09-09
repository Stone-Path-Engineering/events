# Technology Stack

## Framework & Build System
- **Jekyll 4.3.2**: Static site generator for GitHub Pages
- **Ruby**: Runtime environment with Bundler for dependency management
- **Minima theme**: Default Jekyll theme for styling

## Key Dependencies
- `jekyll-feed`: RSS feed generation
- `jekyll-compose`: Content creation helpers
- `webrick`: Local development server

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Start local development server
bundle exec jekyll serve

# Build site for production
bundle exec jekyll build
```

### Content Management
- Posts are created in `_posts/` directory with date-prefixed filenames
- Images stored in `assets/images/`
- Site builds automatically on push to main branch

## Hosting & Deployment
- **GitHub Pages**: Automatic deployment from repository
- **Netlify**: Deploy previews for pull requests
- Custom domain: `iowansofthings.com`

## Third-Party Integrations
- **HubSpot Forms**: Event registration and newsletter signup
- **Microsoft Forms**: Former registration system for some past events