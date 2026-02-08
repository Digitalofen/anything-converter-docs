# Anything Converter

File conversion tool using client-side WASM (FFmpeg) with server-side fallback for complex formats.

## Architecture

### Client-Side (WASM)
- **Images:** Canvas API + WASM libraries
- **Audio/Video:** FFmpeg.wasm (SharedArrayBuffer)
- **Archives:** JSZip, pako

### Server-Side Fallback
- **Documents:** LibreOffice (headless) + Pandoc
- **Complex PDFs:** Ghostscript
- **Hosted:** Private infrastructure (Austria, EU)

Files auto-deleted after 5min.

## Tech Stack
- **Frontend:** Next.js (static export)
- **WASM:** FFmpeg.wasm, custom codecs
- **Backend:** Node.js, LibreOffice, Pandoc
- **Deployment:** Cloudflare CDN

## Privacy
- No uploads for media conversions
- No tracking, no analytics cookies
- GDPR compliant

## Live Demo
https://anythingconverter.com

## License
Proprietary (contact for licensing)
