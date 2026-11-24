# Jus Store v1
A lightweight, mobile-first personal app catalog and launcher. No frameworks or build step.


## Run
Open `index.html` for local preview. For PWA install/offline service worker, host over HTTPS (e.g. GitHub Pages).

## Add/update apps
Edit `apps.js` and add an object to `window.JUS_APPS`. Example:
```js
{ id:'my-app', name:'My App', category:'Productivity', description:'Short description', url:'https://example.github.io/my-app/', version:'1.0.0', icon:'🧰', color:'#5577aa', featured:false }
```
Use unique `id` values. `url:'#'` is a placeholder and displays an alert when opened. Set `featured:true` to display on Home's featured carousel.

## Included
- Search by name, category, description
- Home, Apps, Favorites, Categories and Settings views
- 17 palettes, Solar yellow/black default
- Theme persistence and favorite persistence via localStorage
- Responsive layout, bottom navigation and side drawer
- Basic service-worker caching and manifest

This is a launcher/catalog for web apps and PWAs; it does not install Android APK files.
