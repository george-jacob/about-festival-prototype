# About the festival prototype
Public information about the prototype festival programme app.

* Designing a better solution for digital festival programmes. A learning experience, with the possibility of real use one day.
* Public preview: [festivals-staging.grjacob.com](https://festivals-staging.grjacob.com/)
* Novel user-friendly features for an elevated festival experience, over current competition.
* Progressive web app, works offline.
  
<img width="300" alt="Screenshot_20261110-220039" src="https://github.com/user-attachments/assets/46bfab48-d318-498b-a838-7753ac66bfd2" />

## Closed source, for now
For now, the code is private while the concept is being established.  
Part or all of the project may become open-source in future.  

## Notable features
* Centerpiece: a continuous timeline for a whole multi-venue festival.
* Real location-based weather, sunrise and sunset on the timeline. (More info below.)
* Zoom for detail: pinch and scroll around the timeline, with event detail shown at high zoom.
* Festival-specific colour schemes and timeline customisation options.
* 'Star' the events you want to see and toggle through timeline view modes to see just your plan.

_Coming..._
* Festival map, live info overlays.
* Notifications for schedule changes.
* Messages and updates from festival organisers.
* ...

## Project diary
_N.B. Lag between project progress and diary updates. May be out of date._
[Project diary](https://www.grjacob.com/topics/project-diary-festival-programme-prototype)  
May move in future, e.g. Substack.

## Stack
* UI: React, Node.JS, TypeScript, Vite, Workbox.
* Back end: Google Cloud Run. DB & events TBC.
* Hosting: Google Cloud, Firebase, CloudFlare.
* Testing: Vitest, Playwright
* Other tooling: GitHub (actions), Claude Code.

## Design
Google Material Design (3) is the starting point. Some divergence for novel features.

## Learning objectives
* Full stack, professional-grade setup from scratch (cloud, IaC, CI/CD, etc).
* Claude Code use across a full stack.
* Google Cloud (prior experience only AWS).
* Progressive web apps, React.
* OpenTelemetry.
* Material Design.

## Weather data
Weather forecast data comes from the MET Norway API, which covers the whole world.  
[Met Norway licensing and crediting](https://www.met.no/en/free-meteorological-data/Licensing-and-crediting)  
The prototype app requests weather data from its own back-end service, only for specific festival locations, preventing general misuse. The back-end in turn calls the MET API, but only as needed, to avoid unnecessary load.  

