# Negative Prompts / Anti-Pattern Controls

Use these controls to keep outputs aligned with Art Nouveau aesthetics.

## Master Negative Block

`photorealistic, photo, DSLR, cinematic realism, modern fashion styling, contemporary streetwear, sans-serif logo typography, bold modern headline fonts, UI text overlays, hard cast shadows, high-contrast noir lighting, harsh rim light, noisy gradients, banding artifacts, plastic skin, pore-level hyper-detail skin, beauty-retouch gloss, anime style, chibi proportions, manga screentones, cel-shaded anime eyes, mecha motifs, cyberpunk neon, sci-fi interface elements, low-res, compression artifacts, watermark, signature, malformed hands, extra fingers, distorted anatomy, cluttered background`

---

## Targeted Exclusion Sets

### 1) Block photorealism
`photorealism, photographic texture, camera lens blur, depth-of-field bokeh, realistic skin pores, HDR realism`

### 2) Block modern typography drift
`modern sans-serif, geometric grotesk fonts, corporate branding, minimal Swiss typography, contemporary logo marks`

### 3) Soften lighting character
`hard shadows, hard spotlight, dramatic noir contrast, sharp specular highlights, aggressive rim lighting`

### 4) Reduce noisy gradient artifacts
`grainy gradient noise, color banding, dithering artifacts, over-sharpened transitions, posterization`

### 5) Avoid over-detailed skin rendering
`hyper-detailed skin, pores, blemish microtexture, glossy makeup realism, airbrushed beauty photography`

### 6) Prevent anime drift
`anime, manga, cel shading, chibi, oversized anime eyes, shonen style, kawaii expression exaggeration`

---

## Lightweight Negative (for models sensitive to long negatives)

`photorealistic, modern typography, hard shadows, noisy gradients, hyper-detailed skin, anime/manga style, artifacts, watermark`

## Usage Notes

- If image quality collapses, shorten negatives first.
- Keep anatomy/error terms at the end for diffusion models.
- For MJ/Flux-like systems, prefer concise negatives and stronger positive style anchors.
