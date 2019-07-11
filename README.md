## Steps to reproduce

1. `npm install`
2. `node index.js`

## Expected behaviour

Workbox-build generates a bundle containing the service worker and its dependencies.

## Actual behaviour

Workbox-build generates a bundle containing raw define calls:
`define("./sw.js",["../../../../path/to/my/project/node_modules/workbox-build/node_modules/workbox-precaching/precacheAndRoute.mjs"], function(e) {...})`
