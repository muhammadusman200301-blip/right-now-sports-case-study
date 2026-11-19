# Right Now Sports · Case Study

> **Source code is private under client NDA.** This repo documents the product, the architecture and my role. Happy to walk through it on a call: [book 30 min](https://calendly.com/muhammadusman200301/30min).

**Right Now Sports** is a social sports app. Players challenge each other to 1v1 or ranked battles, host public or invite-only events, stream live, post reels, and find nearby players and events on a map with GPS directions.

| | |
|---|---|
| **My role** | Mobile and full-stack developer |
| **Platforms** | iOS, Android |
| **Live** | [App Store](https://apps.apple.com/us/app/right-now-sports/id6799976756) · [Google Play](https://play.google.com/store/apps/details?id=com.rightnowsports.app) |

## Tech stack
React Native · Firebase (Auth, Firestore, Storage, Cloud Functions) · Firebase Cloud Messaging · Google Maps

## What I built
- Location-based **event discovery** with Google Maps and GPS directions
- **Challenge battles** (1v1 and ranked) and event hosting
- **Reels**, **livestreams** and real-time **messaging**
- **Push notifications** with FCM

## Architecture (simplified)

```
React Native app ──► Firebase Auth
       │
       ├──► Firestore (profiles, events, battles, chats)  ← real-time listeners
       ├──► Storage (reels & media)
       ├──► Google Maps (nearby players & events)
       └──► Cloud Functions ──► FCM push notifications
```

## Challenges and how I handled them
- **Real-time features without a custom server** – used Firestore listeners for chats, battles and events so updates appear instantly.
- **Media-heavy screens on mid-range phones** – paged lists and lazy loading for reels and feeds.

---
More of my work: [Portfolio](https://muhammadusman-portfolio10.netlify.app) · [LinkedIn](https://www.linkedin.com/in/muhammad-usman-987852388/)
