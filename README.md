<h1 align="center">Jellyfin Web with Request Tab</h1>
<h3 align="center">Part of the <a href="https://jellyfin.org">Jellyfin Project</a></h3>

---

<p align="center">
<img alt="Logo Banner" src="https://raw.githubusercontent.com/jellyfin/jellyfin-ux/master/branding/SVG/banner-logo-solid.svg?sanitize=true"/>
<br/>
<br/>
<a href="https://github.com/jellyfin/jellyfin-web">
<img alt="GPL 2.0 License" src="https://img.shields.io/github/license/jellyfin/jellyfin-web.svg"/>
</a>
<a href="https://github.com/jellyfin/jellyfin-web/releases">
<img alt="Current Release" src="https://img.shields.io/github/release/jellyfin/jellyfin-web.svg"/>
</a>
<a href="https://translate.jellyfin.org/projects/jellyfin/jellyfin-web/?utm_source=widget">
<img src="https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-web/svg-badge.svg" alt="Translation Status"/>
</a>
<br/>
<a href="https://opencollective.com/jellyfin">
<img alt="Donate" src="https://img.shields.io/opencollective/all/jellyfin.svg?label=backers"/>
</a>
<a href="https://features.jellyfin.org">
<img alt="Feature Requests" src="https://img.shields.io/badge/fider-vote%20on%20features-success.svg"/>
</a>
<a href="https://matrix.to/#/+jellyfin:matrix.org">
<img alt="Chat on Matrix" src="https://img.shields.io/matrix/jellyfin:matrix.org.svg?logo=matrix"/>
</a>
<a href="https://www.reddit.com/r/jellyfin">
<img alt="Join our Subreddit" src="https://img.shields.io/badge/reddit-r%2Fjellyfin-%23FF5700.svg"/>
</a>
</p>
The point of this Fork is to add a request tab to the Jellyfin Web UI. This tab will allow users to add any website that supports iFrames to it using the plugin:https://github.com/soultaco83/Jellyfin_requests_plugin
![request tab](https://github.com/user-attachments/assets/5bcefd05-eac9-46d0-bdd2-eb87cfa1361b)
![request tab2](https://github.com/user-attachments/assets/611e0411-15c9-4613-8bb5-3d1e024f610f)
![plugin](https://github.com/user-attachments/assets/2c194829-23ea-4029-9eb0-ec239fbf90a7)


Jellyfin Web is the frontend used for most of the clients available for end users, such as desktop browsers, Android, and iOS. We welcome all contributions and pull requests! If you have a larger feature in mind please open an issue so we can discuss the implementation before you start. Translations can be improved very easily from our <a href="https://translate.jellyfin.org/projects/jellyfin/jellyfin-web">Weblate</a> instance. Look through the following graphic to see if your native language could use some work!

<a href="https://translate.jellyfin.org/engage/jellyfin/?utm_source=widget">
<img src="https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-web/multi-auto.svg" alt="Detailed Translation Status"/>
</a>

## Build Process

### Dependencies

- [Node.js](https://nodejs.org/en/download)
- npm (included in Node.js)

### Getting Started

1. Clone or download this repository.

   ```sh
   git clone https://github.com/jellyfin/jellyfin-web.git
   cd jellyfin-web
   ```

2. Install build dependencies in the project directory.

   ```sh
   npm install
   ```

3. Run the web client with webpack for local development.

   ```sh
   npm start
   ```

4. Build the client with sourcemaps available.

   ```sh
   npm run build:development
   ```

## Directory Structure

```
.
└── src
    ├── apps
    │   ├── dashboard     # Admin dashboard app layout and routes
    │   ├── experimental  # New experimental app layout and routes
    │   └── stable        # Classic (stable) app layout and routes
    ├── assets            # Static assets
    ├── components        # Higher order visual components and React components
    ├── controllers       # Legacy page views and controllers 🧹
    ├── elements          # Basic webcomponents and React wrappers 🧹
    ├── hooks             # Custom React hooks
    ├── lib               # Reusable libraries
    │   ├── globalize     # Custom localization library
    │   ├── legacy        # Polyfills for legacy browsers
    │   ├── navdrawer     # Navigation drawer library for classic layout
    │   └── scroller      # Content scrolling library
    ├── plugins           # Client plugins
    ├── scripts           # Random assortment of visual components and utilities 🐉
    ├── strings           # Translation files
    ├── styles            # Common app Sass stylesheets
    ├── themes            # CSS themes
    ├── types             # Common TypeScript interfaces/types
    └── utils             # Utility functions
```

- 🧹 &mdash; Needs cleanup
- 🐉 &mdash; Serious mess (Here be dragons)
