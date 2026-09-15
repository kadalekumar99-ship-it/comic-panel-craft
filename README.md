# Pixazo Sparkle Forge

AI manga/story image generation app built with TanStack Start.

- **Images**: Pixazo API, using a pool of up to 10 keys in parallel.
- **Text**: Z.ai GLM `glm-4.7-flash` (free tier), streamed, one request at a time.

## Configuration

All credentials are stored as server-side secrets and are never shipped to the browser:

| Secret | Purpose |
| --- | --- |
| `PIXAZO_API_KEY_1` … `PIXAZO_API_KEY_10` | Image generation key pool |
| `ZAI_API_KEY` | Z.ai text model key |
| `ZAI_MODEL` | Optional model override (default `glm-4.7-flash`) |

## Development

```sh
bun install
bun run dev
```
