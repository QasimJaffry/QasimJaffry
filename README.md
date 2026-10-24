<p align="center">
  <img src="assets/hero.png" alt="Qasim Hassan, senior software engineer. Mobile and full-stack apps that keep working after launch." width="100%">
</p>

<p align="center">
  <a href="https://qasimjaffry.github.io/qasim-portfolio/"><b>Portfolio</b></a> &nbsp;·&nbsp;
  <a href="https://linkedin.com/in/qasim-hassan-02871a171"><b>LinkedIn</b></a> &nbsp;·&nbsp;
  <a href="https://www.upwork.com/freelancers/~011828438344ce4299"><b>Upwork</b></a> &nbsp;·&nbsp;
  <a href="mailto:qhassan1214@gmail.com"><b>qhassan1214@gmail.com</b></a>
</p>

I build the parts of mobile and web apps that have to keep working after launch: offline sync, subscriptions, sign-in, store receipts and the release pipeline around them. React Native / Expo and React / Next.js, with Firebase, Stripe and RevenueCat behind them. About six years, based in Lahore, open to remote senior roles.

## Shipped

<a href="https://play.google.com/store/apps/details?id=innerverse.app"><img src="assets/card-innerverse.png" alt="Innerverse: a mood journal drawn as a galaxy" width="100%"></a>

**Innerverse.** Every entry becomes a world on a galaxy map drawn with Skia. Design, app, Firebase backend, billing and the Play release are all mine. &nbsp;[Google Play](https://play.google.com/store/apps/details?id=innerverse.app) · [innerverse.app](https://innerverse.app)

<br>

<a href="https://bugmapper.com.tr/"><img src="assets/card-bugmapper.png" alt="BugMapper: scout the tunnels, count the traps" width="100%"></a>

**BugMapper.** Greenhouse staff scan a trap's QR code with the camera, record the count and move on. Counts and photos queue in SQLite and sync when the signal returns; files go to an on-site device over an encrypted transfer. English and Turkish. &nbsp;[bugmapper.com.tr](https://bugmapper.com.tr/)

<br>

<a href="https://agenticly.app"><img src="assets/card-agenticly.png" alt="Agenticly: ask about crypto and stocks" width="100%"></a>

**Agenticly.** Web and mobile client, scheduled agents, Stripe and RevenueCat billing. Built with the team at Stars Computer. &nbsp;[Google Play](https://play.google.com/store/apps/details?id=computer.star.agenticly) · [App Store](https://apps.apple.com/us/app/agenticly-stock-crypto-ai/id6760048191) · [web](https://agenticly.app)

### More

| Product | What I did | Check it |
|---|---|---|
| **Kitty Nip** | Mobile engineer on a live React Native app: upgrades, sign-in, subscriptions, receipt validation in Cloud Functions | [App Store](https://apps.apple.com/us/app/kitty-nip-cat-dating-app/id1520805359) · [Google Play](https://play.google.com/store/apps/details?id=computer.star.kittynip) 10K+ |
| **Safe Deal** | The WebView shopping browser: link handling, loop protection, Zustand state | [Google Play](https://play.google.com/store/apps/details?id=com.safedeal.navigator) 5K+ |
| **Bschedule** (2021 to 2022) | Staff and customer scheduling apps on one API, React Native | Private client tool, apps no longer on the stores |
| **Decidr** | Weighted decision matrices with Stripe. Personal SaaS | [source](https://github.com/QasimJaffry/Decidr) · [live](https://decidr-henna.vercel.app/) |

Client source stays private, so most entries link to the live product instead.

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

<p>
  <img src="https://skillicons.dev/icons?i=react,ts,nextjs,nodejs,firebase,postgres,tailwind,git" alt="React, TypeScript, Next.js, Node.js, Firebase, PostgreSQL, Tailwind, Git" />
</p>

React Native · Expo · Skia · Zustand · Redux Toolkit · SQLite · Stripe · RevenueCat · GitHub Actions
