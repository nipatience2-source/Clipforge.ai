# ClipForge AI

A starter for an AI video web app with a text-to-video and audio-to-video interface, 5-minute project control, and a CapCut-style timeline mockup.

## Run locally
1. Install Node.js 20+.
2. In this folder run `npm install`.
3. Run `npm run dev`.
4. Open `http://localhost:3000`.

## Make generation real
The `/api/generate` route is intentionally a safe integration point. Connect it to a video generation provider you have an account/API key for, then queue long jobs on a server-side worker. Use FFmpeg to assemble generated clips, audio, captions and transitions into the final MP4.

Do not expose provider API keys in browser code.

## Production roadmap
- Authentication/database/storage: Supabase or Firebase.
- AI generation: connect your chosen video API.
- Speech-to-text for audio projects.
- Server-side rendering/FFmpeg worker for 5-minute exports.
- Object storage for source and output files.
- Usage credits and payments.
- Rate limits, moderation, retries, job queue and logging.
- Deploy frontend on Vercel or another Node host; deploy long-running workers separately.

This is a working UI/API starter, not a finished production video-generation service. Provider APIs and pricing change, so configure those separately.
