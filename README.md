# Hey, I'm Josh 👋

I'm a senior frontend engineer. Vue and Nuxt are home, but I'm just as comfortable in React and Next.js, and lately a big chunk of my time goes into AI development: building with tools like Claude Code, wiring up MCP servers, and figuring out where AI actually earns its place in a product versus where it's just a buzzword.

The short version of my story: my family and I spent a stretch living full-time in an RV, towing a fifth wheel cross-country with two dogs and a truck I'd never towed anything with before. I wrote code from campgrounds with questionable Wi-Fi. We've since parked it for good and just moved to Portland, and the Wi-Fi is a lot better.

I do my best thinking early in the morning before anyone else is up. That's usually when the side projects happen. There are a few of them.

---

## 🗺️ Roam Planner
**<a href="https://roamplanner.net" target="_blank" rel="noopener noreferrer">roamplanner.net</a>** · live

`Vue 3` · `Pinia` · `Supabase` · `Leaflet` · `Netlify Functions` · `Vitest` · `Storybook`

I built this because I needed it. Planning an RV route is not the same as planning a road trip. You care about where you can actually fit a big rig, how far you can drive before you hate yourself, and which campground actually has a site open. I was solving that by hand every week, so I wrote an app for it. It's been live for months now.

What's under the hood:

- **A real backend-for-frontend.** 13 Netlify serverless functions handle routing, geocoding, weather, fuel prices, park data and campground search. API keys stay server-side and never ship to the browser. Routing uses OpenRouteService with a keyless OSRM fallback, so the app degrades instead of breaking.
- **Accounts and data on Supabase**, with 40+ migrations behind it. That covers trips, favorites, friends and scheduled email reminders for upcoming stays.
- **Interactive maps** built on Leaflet with marker clustering, so a map full of parks doesn't melt your phone.
- **A proper design system**, organized as atoms, molecules and organisms, with ~70 Storybook stories and an accessibility addon checking them.
- **100+ test files** in Vitest, plus Sentry for errors and PostHog for product analytics.
- **Versioning based on user impact.** The dev changelog is generated from commit history, and users get a separate, hand-curated "What's new."

It also hands out badges for parks you visit. Engineers need fun too.

Built AI-assisted with Claude Code, which taught me a lot about steering an AI through a real codebase: where it needs guardrails, and where it just flies.

---

## 🎮 Retro Gamer Lofi
**<a href="https://retrogamerlofi.com" target="_blank" rel="noopener noreferrer">retrogamerlofi.com</a>**

`Nuxt 3` · `TypeScript` · `Nitro` · `Netlify Blobs` · `Vitest`

This is the home base for my lofi remixes of classic game soundtracks. I didn't want another scrolling marketing page, so the whole site is a PS1-style console shell. You pick a station from a carousel on the home screen and drop into a focused workspace for music, videos, merch or a community voting board.

Engineering bits I'm proud of:

- **Built for the keyboard, not just tolerant of it.** You can navigate the whole thing like a console: arrow keys through libraries, Enter to activate, focus-trapped modals that return focus to where you came from, and skip links. Touch and swipe work too, and swipes are tuned so they don't route you somewhere by accident.
- **Nuxt server routes** that pull from YouTube, Spotify and the Fourthwall store API. Every surface has a fallback, so if a provider goes down the page stays usable.
- **A voting API** where fans request the next game to remix. It validates email, rate-limits with an IP sliding window, treats repeat votes as no-ops, keeps emails server-side only, and stores everything in Netlify Blobs.
- **SEO done properly:** JSON-LD, a generated sitemap and canonical metadata.
- **It respects `prefers-reduced-motion`,** plus there's a comfort mode for anyone who wants less going on.

---

## 📟 Real Pokédex
**<a href="https://aprettydecentpokedex.netlify.app/" target="_blank" rel="noopener noreferrer">Live demo</a>** · <a href="https://github.com/jmart790/real-pokedex" target="_blank" rel="noopener noreferrer">Source</a>

`Vue 3` · `TypeScript` · `Pinia` · `PokeAPI` · `Sass`

Everyone builds a Pokédex at some point. I wanted mine to feel like a device you could pick up off the desk, so it's a realistic Nintendo Switch-inspired shell with typed data from PokeAPI behind it.

This is the project where I really fell for CSS. I lost a lot of sleep on it. It almost never left my laptop, and the only reason it shipped is that a friend kept bugging me until I put it out there.

---

## 🚧 joshcodesthings2024
**<a href="https://github.com/jmart790/joshcodesthings2024" target="_blank" rel="noopener noreferrer">Source</a>** · desktop-only proof of concept

`Vue 3` · `TypeScript` · `GSAP`

My portfolio. I started it in 2024. It is not 2024 anymore.

This is my third or fourth attempt, and this time it's a Mega Man X tribute. You don't scroll through a résumé, you pick a stage. There's a stage select screen, a work history page that plays like a game screen, a jukebox, an art gallery, a rotating About Me cube, a password screen (every good Mega Man game had one) and a mystery page I'm not going to explain.

So why isn't it done? Every time I get close, I have a new idea and tear something down. Engineers can build anything, and that's exactly the problem, because nothing tells you when to stop. This project is my long-running and very personal proof of why designers matter. A good one would have locked this down two years ago.

It'll ship eventually. Probably as joshcodesthings2027.

---

## 🧰 What I work with

- **Frontend:** Vue, Nuxt, React, Next.js, TypeScript, Pinia, Sass, and a lot of hand-written CSS
- **Backend-ish:** Supabase, Netlify Functions, Nitro server routes, Postgres migrations
- **Quality:** Vitest, Vue Test Utils, Storybook, accessibility as a default rather than a ticket
- **Observability:** Sentry, PostHog
- **AI development:** Claude Code for day-to-day building, plus a custom MCP server I wrote so AI can drive DaVinci Resolve

## 🕹️ Off the clock

Retro games, always. Getting to know Portland after a long stretch of never staying anywhere. Trying to make my family laugh, with mixed results.

---

> *If you've read this far, you're either hiring or you also have an unfinished portfolio. Either way, hi.*
