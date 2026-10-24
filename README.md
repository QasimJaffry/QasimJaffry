# Qasim Hassan

I build the parts of mobile and web apps that have to keep working after launch: offline sync, subscriptions, sign-in, store receipts and the release pipeline around them. React Native / Expo and React / Next.js, with Firebase, Stripe and RevenueCat behind them.

Lahore (UTC+5) · about six years · open to remote senior roles

[Portfolio](https://qasimjaffry.github.io/qasim-portfolio/) · [LinkedIn](https://linkedin.com/in/qasim-hassan-02871a171) · [Upwork](https://www.upwork.com/freelancers/~011828438344ce4299) · qhassan1214@gmail.com

---

## Best work

**Agenticly.** AI research assistant for crypto and stocks. I built the React Native app and web client, the scheduled-agents feature and the Stripe and RevenueCat billing that decides who may run an agent. Built with the team at Stars Computer.
[Google Play](https://play.google.com/store/apps/details?id=computer.star.agenticly) (10K+) · [App Store](https://apps.apple.com/us/app/agenticly-stock-crypto-ai/id6760048191) · [web](https://agenticly.app)

**Kitty Nip.** A live React Native app with 10K+ downloads that I've maintained and extended since late 2023: Google, Apple and phone sign-in, subscription plans and restore purchase, Android receipt validation in a Cloud Function, converting legacy class components, and the upgrade to React Native 0.79.
[Google Play](https://play.google.com/store/apps/details?id=computer.star.kittynip) (10K+) · [App Store](https://apps.apple.com/us/app/kitty-nip-cat-dating-app/id1520805359)

**Innerverse.** A mood journal drawn as a galaxy, rendered with Skia. I did all of it: design, the React Native app, the Firebase backend, billing and the Play release.
[Google Play](https://play.google.com/store/apps/details?id=innerverse.app) · [innerverse.app](https://innerverse.app)

Client source stays private, so these link to the live products.

## More

| Product | What I did | Check it |
|---|---|---|
| **BugMapper** (2023 to now, contract) | The field app for a greenhouse pest-scouting platform: camera QR scanning, offline SQLite queue with sync, encrypted file transfer with an on-site device, English and Turkish | [bugmapper.com.tr](https://bugmapper.com.tr/) |
| **Safe Deal** | Contributor on the WebView shopping browser (Oct to Nov 2024): moved state from Redux and Context to Zustand, reworked data fetching with React Query, fixed a navigation loop | [Google Play](https://play.google.com/store/apps/details?id=com.safedeal.navigator) 5K+ |
| **Bschedule** (2021 onward) | Staff and customer scheduling apps on one API, React Native. Built the admin app and upgraded it to React Native 0.73 in 2026 | Private client tool |
| **Decidr** | Weighted decision matrices with AI scoring and a reasoning trace. Personal project: Next.js, Supabase | [live](https://decidr-henna.vercel.app/) |

## What I'm usually asked to fix

- Subscriptions that grant or revoke access wrongly across Stripe, RevenueCat, Apple and Google
- Offline-first apps that lose or duplicate data when the connection returns
- Auth and onboarding flows that break on one platform only
- React Native upgrades on apps that started life as class components

## Working notes

- **Do entitlement writes on the server.** In Innerverse the premium flag is written only by a RevenueCat webhook, with tests; Firestore rules refuse client writes to it. Webhook handlers are idempotent so a retried event cannot double-grant.
- **Queue first, sync later.** In BugMapper every count and photo lands in a local SQLite queue with a visible pending list, so a tunnel with no signal loses nothing.
- **Validate store receipts yourself.** Kitty Nip checks Android purchases against the Play Developer API from a Cloud Function instead of trusting the client.

## Stack

React Native, Expo, Skia, Zustand, SQLite · React, Next.js, TypeScript, Tailwind · Firebase, Cloud Functions, Node.js, PostgreSQL · Stripe, RevenueCat · GitHub Actions, EAS Build
