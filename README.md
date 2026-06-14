# TechCon 2024 Conference Landing Page

A semantic, lightweight HTML5 landing page scaffolded for the TechCon 2024 conference platform. This codebase serves as the entry point application template, establishing core site architecture, internationalization support, and responsive viewport mapping.

##  Key Features

* **Semantic HTML5 Layout**: Structured via descriptive tags (`<header>`, `<nav>`, `<main>`, `<section>`) to optimize search engine crawling and screen reader accessibility.
* **Global Configuration**: Configured with `lang="en"` and standard UTF-8 character encoding to handle universal text formatting without degradation.
* **Responsive Architecture**: Implements standard viewport metadata tags ensuring fluid layout scalability across distinct desktop, tablet, and mobile device profiles.
* **Native Media Integration**: Embeds native HTML5 `<video>` player blocks backed by assistive `<track>` configurations for closed captioning and multi-language subtitle streams.

##  File Infrastructure

The baseline structure maps the primary routing links to independent system modules:

```text
├── index.html        # Main landing page & video portal
├── about.html        # Conference vision, speakers, and background
├── schedule.html     # Chronological timeline of technical tracks
├── register.html     # Attendance, ticketing, and registration form
└── contact.html      # Helpdesk, venue tracking, and maps
```

## 🛠️ Implementation Requirements

To transition this blueprint into active production, developers must configure the media playback attributes within the `<main>` container:

1. **Video Source Mapping**: Update the `<source>` tag `src` path to point directly to your hosting directory (e.g., `assets/videos/promo.mp4`) and declare its correct MIME type signature (e.g., `type="video/mp4"`).
2. **WebVTT Configuration**: Bind functional `.vtt` asset paths to the `<track>` element `src` selector to fully render functional subtitles for user accessibility tools.
