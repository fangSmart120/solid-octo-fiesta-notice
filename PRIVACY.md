# Privacy Policy

**Effective date:** 2026-08-10
**Applies to:** Claw (working name), an iOS workout playlist generator, part of the solid-octo-fiesta project.

This policy describes what data the app processes, where it is processed, and what we never collect. It applies to the current closed-testing (TestFlight) phase and will be updated before public release.

## The short version

- **Health data never leaves your device.** Ever.
- We do not require an account, do not run ads, do not use tracking/analytics SDKs, and do not sell data.
- We store only what the core feature needs: your playlist requests, preferences, and feedback.

## Data processed on your device only

The following data is read and processed **exclusively on your device** and is never transmitted to our servers or any third party:

- **Apple Health (HealthKit) data** — if you grant permission: sleep duration, resting heart rate trends, and recent workout history. These are used solely to compute a readiness score (0–100) on-device, which maps to an energy level (1–10). **Only the resulting energy level number is ever sent** — never the underlying health data.
- Your Apple Music library and listening data (accessed via MusicKit, governed by Apple's own privacy policy).

## Data sent to our backend

To generate playlists, the app sends:

| Data | Why |
|------|-----|
| Workout request parameters (workout type, duration, energy level, music preferences such as genre/language/explicit-content settings) | Required to generate a playlist |
| Anonymous device identifier | Distinguishes your preferences and history without an account |
| Generated playlist history (song titles/artists) | Lets you revisit past playlists in the app |
| Feedback events (song likes/dislikes) | Improves your future recommendations |

## Third-party processors

- **Apple Music API** — music metadata and playback (Apple's privacy policy applies).
- **OpenAI API** — LLM playlist generation. Requests may include your workout parameters and music preferences, never health data.
- **GetSongBPM.com** — song tempo/key metadata lookups. No user data is sent; lookups contain only song titles and artists.

## What we never do

- No accounts, emails, or phone numbers collected.
- No advertising, no ad networks, no analytics/tracking SDKs.
- No sale or sharing of personal data with data brokers.
- No collection of precise location. (If you choose to auto-detect your region for localized charts, the region code is derived on-device and raw location is discarded.)
- No server-side storage of health data, under any circumstance.

## Data retention & deletion

Playlist history and preference data are retained to provide the app's core features. Because data is tied to an anonymous device identifier, you can request deletion by opening an issue in this repository (see [SUPPORT.md](SUPPORT.md)) and we will guide you through identifying and deleting your records.

## Children

The app is not directed at children under 13 and does not knowingly collect their data.

## Changes

Material changes to this policy will be committed to this repository with a new effective date.

## Contact

See [SUPPORT.md](SUPPORT.md).
