# Qasim Hassan

I build the parts of mobile and web apps that have to keep working after launch: offline sync, subscriptions, sign-in, store receipts and the release pipeline around them. React Native / Expo and React / Next.js, with Firebase, Stripe and RevenueCat behind them.

Lahore (UTC+5) · about six years · open to remote senior roles

[Portfolio](https://qasimjaffry.github.io/qasim-portfolio/) · [LinkedIn](https://linkedin.com/in/qasim-hassan-02871a171) · [Upwork](https://www.upwork.com/freelancers/~011828438344ce4299) · qhassan1214@gmail.com

---

## Shipped

Each row says what I did and where you can check it. Client source stays private, so most rows link to the live product.

| Product | My part | Check it |
|---|---|---|
| **Innerverse** | Everything: design, React Native app, Firebase backend, billing, Play release. A mood journal drawn as a galaxy, rendered with Skia | [Google Play](https://play.google.com/store/apps/details?id=innerverse.app) · [innerverse.app](https://innerverse.app) |
| **BugMapper** (2023 to now) | Senior engineer on a greenhouse pest-scouting platform. The field app: camera QR scanning, offline SQLite queue with sync, encrypted file transfer with an on-site device, English and Turkish | [bugmapper.com.tr](https://bugmapper.com.tr/) |
| **Agenticly** | Web and mobile client, scheduled agents, Stripe and RevenueCat billing. Team product, Stars Computer | [Google Play](https://play.google.com/store/apps/details?id=computer.star.agenticly) 10K+ · [App Store](https://apps.apple.com/us/app/agenticly-stock-crypto-ai/id6760048191) · [web](https://agenticly.app) |
| **Kitty Nip** | Mobile engineer on a live React Native app: upgrades, sign-in, subscriptions, receipt validation in Cloud Functions | [App Store](https://apps.apple.com/us/app/kitty-nip-cat-dating-app/id1520805359) · [Google Play](https://play.google.com/store/apps/details?id=computer.star.kittynip) 10K+ |
| **Safe Deal** | The WebView shopping browser: link handling, loop protection, Zustand state | [Google Play](https://play.google.com/store/apps/details?id=com.safedeal.navigator) 5K+ |
| **Bschedule** (2021 to 2022) | Staff and customer scheduling apps on one API, React Native | Private client tool, apps no longer on the stores |
| **Decidr** | Weighted decision matrices with Stripe. Personal SaaS | [source](https://github.com/QasimJaffry/Decidr) · [live](https://decidr-henna.vercel.app/) |

## What I'm usually asked to fix

- Subscriptions that grant or revoke access wrongly across Stripe, RevenueCat, Apple and Google
- Offline-first apps that lose or duplicate data when the connection returns
- Auth and onboarding flows that break on one platform only
- React Native upgrades on apps that started life as class components

## Working notes

Short, from real work.

- **Do entitlement writes on the server.** In Innerverse the premium flag is written only by a RevenueCat webhook, with tests; Firestore rules refuse client writes to it. Webhook handlers are idempotent so a retried event cannot double-grant.
- **Queue first, sync later.** In BugMapper every count and photo lands in a local SQLite queue with a visible pending list, so a tunnel with no signal loses nothing.
- **Validate store receipts yourself.** Kitty Nip checks Android purchases against the Play Developer API from a Cloud Function instead of trusting the client.

## Stack

<img src="https://skillicons.dev/icons?i=react,ts,nextjs,nodejs,firebase,postgres,tailwind,git" alt="React, TypeScript, Next.js, Node.js, Firebase, PostgreSQL, Tailwind, Git" />

React Native · Expo · Skia · Zustand · Redux Toolkit · SQLite · Stripe · RevenueCat · GitHub Actions
