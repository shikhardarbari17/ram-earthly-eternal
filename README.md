# RAM - Earthly and Eternal
### An Interactive Digital Children's Book

**Live demo:** https://capable-babka-bff8db.netlify.app

A premium interactive storybook adapting Dr. Shikha Darbari's *Ram: Earthly and Eternal* for children aged 6-10. Built entirely with vanilla HTML, CSS, and JavaScript — no frameworks.

---

## What it is

A 14-chapter animated values-education journey based on the Ramayan, designed for children, parents, temples, schools, and cultural centres. Chapter 1 is fully built and live.

**Educational loop:** Story - Interaction - Reflection - Badge - Next Chapter

---

## Features (Chapter 1)

- Animated cover with full-bleed cinematic video scenes (Runway ML Gen-4)
- 5 story pages with Hindi verse cards and Web Speech API narration
- Interactive "Four Powers of Ram" cards with SVG sand-drawing animation
- **Ram's Golden Arrow** — HTML5 Canvas archery game with projectile physics, pass-through hit detection, particle effects, and a pass/fail gate (score 3+ to continue)
- Community permission system with privacy-first consent architecture
- Reflection exercises with a 80-word-limit writing canvas and a drawing tool
- Progress tracking via localStorage
- Supabase (PostgreSQL) backend for community submissions with 3-layer noise filtering and row-level security

---

## Games built

### Ram's Golden Arrow (Chapter 1)
HTML5 Canvas game. Aim with mouse, shoot 3 arrows. Arrows pass through targets enabling chain hits. Natural projectile arc with gravity. Dotted trajectory preview. Particle burst on hit. Pass gate: 3+ targets required to proceed.

### Hanuman's Great Leap (Chapter 7)
Side-scrolling runner. Spacebar/tap to jump over rock obstacles. Collectible Sanjeevani herb plants add score. One life - hit a rock and restart. At journey end, Hanuman must jump for the final Sanjeevani Booti to win. Celebration finale: Hanuman flies upward with expanding golden particle rings, radial sunburst, and "Jai Hanuman!" text reveal.

---

## Tech stack

- **Frontend:** Vanilla HTML5, CSS3, JavaScript (no frameworks)
- **Canvas games:** HTML5 Canvas 2D API, custom physics engine
- **Database:** Supabase (PostgreSQL) with RLS policies
- **Storage:** Supabase Storage (drawings), YouTube (video streaming)
- **Hosting:** Netlify
- **AI video:** Runway ML Gen-4, Higgsfield
- **Audio:** Web Speech API (Hindi hi-IN narration)

---

## Architecture

Single HTML file per chapter (~470KB). Shared design system (fonts, colours, animations) defined in embedded CSS. All game logic, TTS, Supabase integration, and navigation in embedded vanilla JS. Videos streamed from YouTube. Drawings uploaded to Supabase Storage.

**Design tokens:** Cream `#FFFBF2` - Saffron `#F97316` - Gold `#D97706` - Deep Brown `#3B1A08` - Jade `#059669` - Lotus `#E11D48`

---

## Roadmap

- **Phase 2:** Chapters 2-4 + Ram's Journey interactive India map
- **Phase 3:** Chapter 7 with Hanuman's Great Leap embedded
- **Phase 4:** Dharma Rath Builder (Ch9) + Ravan's Inner Enemies (Ch10)
- **Phase 5:** Pearl collector, badges, Dharma Certificate, parent/teacher guide

---

*Adapted from the original work by Dr. Shikha Darbari, published by Prabhat Prakashan.*
