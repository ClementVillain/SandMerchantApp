# Sand Merchant — Digital Advent Calendar

**A story-driven digital Advent calendar themed around the film *Rise of the Guardians*, prototyped in a four-day university workshop.**
The player explores their character's bedroom and follows the Sandman's story chapter by chapter, one chapter per day of Advent.

> University workshop — IUT de Lannion, BUT MMI. Built 16–19 December 2025.

---

## Features

- **Illustrated onboarding**: an intro sequence that leads into the character's bedroom.
- **Interactive bedroom hub**: wardrobe, story book and bed, each opening its own scene.
- **Chapter list**: the story's chapters (titles written for the calendar), with the first chapter playable.
- **Wardrobe**: dress up the character by layering clothing items (hats and more) over the illustration.
- **Supabase authentication** (sign-up and login), implemented then left out of the final workshop build.

The interface is in French.

---

## Tech stack

| Area | Technology |
|---|---|
| Framework | React 19 + Vite |
| Routing | Raviger |
| UI | Radix UI Themes + Radix Icons |
| State | Nanostores |
| Backend / Auth | Supabase |

---

## Project structure

```
SandMerchantApp/packages/_app/
├── src/
│   ├── FirstConnexion/   # Intro sequence and first visit to the bedroom
│   ├── Home/             # Bedroom hub (wardrobe, chapters, bed)
│   ├── Connexion/        # Login and sign-up (Supabase)
│   └── App.jsx           # Routes
├── base/components/      # Chapter, chapter list, wardrobe, bed, speech bubbles
└── util/supabase.js      # Supabase client
```

---

## Getting started

```bash
cd SandMerchantApp/packages/_app
npm install
npm run dev
```

Create a `.env` file in `SandMerchantApp/packages/_app/`:

```env
VITE_PUBLIC_SUPABASE_URL=<your_supabase_url>
VITE_PUBLIC_SUPABASE_KEY=<your_supabase_public_key>
```
