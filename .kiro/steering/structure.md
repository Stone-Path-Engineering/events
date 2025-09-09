# Project Structure

## Core Jekyll Structure
- `_config.yml`: Site configuration and settings
- `_posts/`: Event announcements with date-prefixed filenames (YYYY-MM-DD-title.md)
- `_layouts/`: Page templates (homepage.html extends default)
- `_includes/`: Reusable components (header.html, footer.html)
- `_site/`: Generated static site (ignored in git)

## Content Organization
- `index.md`: Homepage with upcoming/past events
- `about.md`: Host information and sponsorship details
- `past-events.html`: Archive of previous events
- `assets/images/`: Event banners, logos, icons, and sponsor images

## Post Categories & Conventions
- **Categories**: `[event, hardware_hangout|firmware_fellowship, next|past]`
- **"next"**: Current upcoming event (only one should exist)
- **"past"**: Previous events for archive display
- **Permalinks**: Use format `/hh-month-year` or `/ff-month-year`

## Front Matter Requirements
```yaml
layout: post
title: Event Name - Month Year
date: YYYY-MM-DD HH:MM:SS -0600
categories: [event, event_type, status]
excerpt_separator: <!--more-->
permalink: /event-slug
```

## Content Structure Pattern
1. Banner image
2. Date/time/location details
3. Event description with `<!--more-->` break
4. Event highlights, audience, agenda
5. Registration form (HubSpot or Microsoft Forms)
6. Sponsor logos and links
7. Additional details (parking, etc.)

## Image Naming Conventions
- Banners: `banner_event_type_YYYY_MM.png`
- Icons: `icon_event_type.png`
- Logos: Descriptive names with organization