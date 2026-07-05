website link : https://cutout-psi.vercel.app/
# Cutout — background remover

A single-file webpage that removes image backgrounds entirely in your browser. No server, no upload, no dependencies.

## How it works

It uses color-distance matching (a chroma-key technique, like a green screen), not AI segmentation. Every pixel is compared to the reference background color; close matches become transparent, distant ones stay opaque, with a soft blend in between.

## Best results

- Solid or plain backgrounds (white walls, seamless paper, product shots, ID photos, logos)
- Even lighting, no heavy shadows on the background

## Limitations

- Won't cleanly separate a subject from busy, textured, or multi-colored backgrounds
- If the subject shares a color with the background, that part may get cut too
- Very large images are auto-scaled down (max 1400px) for performance
