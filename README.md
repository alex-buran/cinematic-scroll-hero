# MOTION · Cinematic Scroll Hero · Landing Page Concept

**▶ Live demo: https://alex-buran.github.io/cinematic-scroll-hero/**

A landing page concept built around one hand-written WebGL fog and light
shader, raymarched live in the browser. There is no video and no image
sequence: the whole scene is computed on the GPU, and it reacts to scroll
and cursor movement.

## What it does

- **Procedural scene.** One raymarched fog volume with volumetric light
  shafts and drifting dust, built from 3D noise. No textures, no footage.
- **Scroll-driven color mood.** A cosine palette shifts the color
  continuously across the whole page, with no hard cuts between sections.
- **Smoothed input.** Scroll and mouse positions are eased before they
  reach the shader, so the camera drifts instead of snapping.
- **Built for real devices.** The scene renders at reduced resolution and
  the browser upscales it, which keeps it smooth on laptops and phones. A
  grain overlay hides the softness and adds to the film look.
- **Cinematic framing.** Letterbox bars on wide screens, hidden
  automatically on tall and mobile screens.
- **Interaction details.** Custom cursor, magnetic call-to-action button,
  staggered section reveals, and a preloader that settles into the scene.

## Tech

- One self-contained `index.html`, no build step
- Three.js (r128, from cdnjs) for the WebGL context, with a custom GLSL
  fragment shader for the scene
- Vanilla HTML / CSS / JavaScript
- Google Fonts (Bricolage Grotesque, Inter)
- Responsive layout; if the Three.js CDN fails, the preloader still clears

## Design & build

Designed and built by **[Softburn.tech](https://softburn.tech)**.
