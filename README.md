# pineapple-press — free cloud audio compression behind Pineapple.

One workflow: `compress.yml` (ffmpeg → Opus 64k stereo).

Used by the Pineapple Android app and the Pineapple Telegram bot through
the `thorfin-relay` Cloudflare worker (target `press`), which owns the
GitHub token server-side. Clients only pass `{audio_url, job_id, ext}`.
