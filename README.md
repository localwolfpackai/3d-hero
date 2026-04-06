# 3D Hero

> Scroll-responsive WebGL hero section with dithered black and white aesthetics.

A full-screen canvas experiment where 3D cubes morph through L, U, P, O letterforms as you scroll. Uses a 4x4 Bayer dithering shader for a high-contrast film look, with glassmorphism content sections layered over the fixed canvas.

## Quick start

```bash
git clone https://github.com/localwolfpackai/3d-hero.git
cd 3d-hero
npm install
npm run dev
```

## How it works

1. **Hero section** -- full-screen canvas with dithered LUPO animation
2. **Scroll trigger** -- letters cycle based on scroll depth
3. **Text sync** -- "move" word drops and vanishes on an 8-second cycle
4. **Content sections** -- glassmorphism panels scroll over the fixed canvas

## Stack

- **Phenomenon.js** -- lightweight WebGL renderer (2kB)
- **Vite** -- dev server with HMR
- **Custom shaders** -- Bayer dithering, morphing geometry
- **CSS keyframes** -- text entrance animations

## Structure

```
3d-hero/
├── index.html          # Page with hero + content sections
├── src/
│   ├── main.js         # WebGL animation + scroll logic
│   └── styles.css      # Layout + animations
└── package.json
```

## License

MIT -- Lupo Studios
