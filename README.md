# Moggr

Free PSL face rating + glow-up coach for Android. No account, no paywall, no cloud. Your photos never leave your phone.

## How it works

1. Watch the intro, answer 5 quick questions.
2. Scan your face from 3 angles (front, left, right) with on-screen guides.
3. Get your PSL score (1–8: LTN / MTN / HTN / Chadlite / Chad) plus what to fix first.
4. Ask Moggr Coach anything.

## The rating

The app measures 15 facial features on-device (ML Kit, bundled model, no network) — symmetry, facial thirds, fifths, midface ratio, eye spacing, FWHR, jawline, chin, cheekbones, side profile and more. Every number comes from landmark geometry, not vibes.

The 1–8 tiers are community conventions from looksmaxxing forums, not science. Moggr reports them straight — a real number, not a participation trophy.

| Score | Tier |
|---|---|
| 7.75+ | Gigachad |
| 7.0–7.74 | Chad |
| 6.0–6.99 | Chadlite |
| 5.0–5.99 | HTN — High Tier Normie |
| 3.0–4.99 | MTN — Mid Tier Normie |
| 1.4–2.99 | LTN — Low Tier Normie |
| < 1.4 | Sub-5 |

## Privacy

- **Face scan:** 100% on-device. Photos are processed on your phone and never uploaded. No account exists to tie them to.
- **Coach chat:** runs on a free keyless chat API, so your typed questions go to that API. If you attach a photo in the coach tab, it's scanned on your phone and only the measurements as text are sent — the image itself never leaves your device.

## Install

Download the APK from https://kurupdevs.github.io/moggr/, open it, allow "install unknown apps" if asked. Done, no signup.

## Permissions

- Camera — the 3 scan angles. Nothing else.
- Internet — only the Coach chat tab. The scan never uses the network.

## Be real with yourself

- Ratings are photo-dependent estimates. Lighting, angle, expression all move the number. Same face, different photo, different score.
- Community ratios (FWHR, ESR, "ideal" thirds) are forum consensus, not peer-reviewed science.
- The coach is a free chatbot — it can be slow, it's guidance not professional advice, and it'll never recommend surgery.
- Moggr is not a medical device. If you're struggling with how you look, talking to a real person you trust beats any rating.

A number from your camera doesn't decide your worth. Use it for the stuff you can control — skin, hair, fitness, style — and log off when it stops being useful.

## Build it yourself

Android Studio, JDK 17:

```
./gradlew assembleRelease
```

Release signing needs the keystore, which isn't in this repo.

## Built with

Kotlin + Jetpack Compose, CameraX, ML Kit face detection (on-device), OkHttp.

## License

MIT. Maintained by [kurupdevs](https://github.com/kurupdevs).
