# Spot Me

A shared workout log for two training partners.

- Log sessions as exercises with weight × reps sets (lb)
- Head-to-head board of each lifter's best estimated 1RM (Epley) per lift
- Progress chart of estimated 1RM over time, per lifter
- PR badges on sets that beat a lifter's previous best

## Installable app (`docs/`)

A home-screen app (PWA) hosted on GitHub Pages, synced through Firebase. Works offline at the gym and syncs when signal comes back.

**App URL:** https://ezcheezy1.github.io/Claude/

### One-time setup

1. **GitHub Pages:** repo Settings → Pages → Source "Deploy from a branch" → branch `claude/workout-tracking-app-0lqtep`, folder `/docs` → Save.
2. **Firebase project:** at https://console.firebase.google.com, Add project (Analytics off).
3. **Sign-in:** Build → Authentication → Get started → Email/Password → Enable. Then Authentication → Settings → Authorized domains → Add `ezcheezy1.github.io`.
4. **Database:** Build → Firestore Database → Create database → production mode.
5. **Rules:** Firestore → Rules → paste `docs/firestore.rules` with both of your emails in the crew list → Publish.
6. **Config:** Project settings (gear) → Your apps → Web (`</>`) → register the app, then copy `apiKey`, `authDomain`, `projectId`, `appId` into `docs/config.js`.

### Install on a phone

- **iPhone:** open the app URL in Safari → Share → Add to Home Screen.
- **Android:** open it in Chrome → ⋮ → Install app.

## claude.ai version (`index.html`)

The original artifact: https://claude.ai/artifact/QQFpdW6DCtxeUvWf13zmoG. It syncs through the Claude artifact database, which only lets people inside the owner's account write.
