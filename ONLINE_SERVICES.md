# Online multiplayer, chat and voice — implementation roadmap

This repository currently contains a static browser prototype. The controls and UI are not a working online service.

1. **Accounts / friends / persistent chat:** use Supabase or Firebase with secure database rules, authentication, blocking/reporting and rate limits.
2. **Live game sessions:** use an authoritative game server or multiplayer provider to synchronize player movement, combat, pickups, match state and disconnects. Do not trust clients to decide damage or rewards.
3. **Voice:** use a WebRTC SFU or dedicated voice provider plus signaling. Implement microphone permission, team channels, push-to-talk, mute/deafen and moderation.
4. **Deployment:** GitHub Pages is for the static web client; deploy backend/server separately.
5. Never commit service-role keys, admin credentials or private keys into the repository.
