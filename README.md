# ASCII Image Reveal on Scroll

A scrollable image gallery where each photo loads as an animated ASCII art grid before revealing the full image.

## Preview

Images start hidden behind a canvas. Each cell appears in a shuffled order with a scramble effect on darker regions, then the real photo fades in once the ASCII animation completes.

## Features

- Converts images to ASCII using brightness sampling on a canvas grid
- Staggered cell animation with random scramble on dense (dark) areas
- Responsive masonry-style gallery layout
- Built with vanilla JavaScript — no framework required

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or later recommended)

### Install

```bash
npm install
```

### Run locally

```bash
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

## Project Structure

```
├── index.html      # Gallery markup
├── script.js       # ASCII conversion and reveal animation
├── styles.css      # Grid layout and reveal states
└── public/         # Sample images (img1.jpg – img15.jpg)
```

## Configuration

Tune the effect in `script.js`:

| Constant | Default | Description |
|----------|---------|-------------|
| `ASCII_CHARS` | `........:::=+xX#0369` | Character set from light to dark |
| `ASCII_COLUMNS` | `25` | Grid width in characters |
| `IMAGE_STAGGER_MS` | `100` | Delay between each image starting |
| `CELL_APPEAR_MS` | `2` | Delay between each cell appearing |
| `SCRAMBLE_COUNT` | `10` | Scramble iterations for dark cells |

## Author

**AJ** — [anassjid.dev](https://anassjid.dev)

## License

ISC
