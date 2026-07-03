# ECO AIR SERVICE — Corporate Website

## [TECH_STACK]
- **Framework:** Next.js 16.2.10 (App Router)
- **UI Library:** React 19.2.7
- **Styling:** Tailwind CSS 4.3.2
- **Animation:** Framer Motion 12.42.2
- **Language:** TypeScript 6.0.3
- **Fonts:** Inter, Manrope (via next/font)

## [ARCHITECTURE]
```
eco-air-service/
├── src/
│   ├── app/             # Next.js App Router pages (11 routes)
│   ├── components/
│   │   ├── ui/          # Design system (Button, Card, Badge, Input, etc.)
│   │   ├── layout/      # Header, Footer, MobileMenu
│   │   └── sections/    # Hero, TrustedBy, PartnerBrands, Services, etc.
│   ├── lib/             # data.ts, images.ts, utils.ts
│   └── types/           # TypeScript interfaces
├── next.config.ts
├── package.json
└── PROJECT_MAP.md
```

## [SYSTEM_FLOW]
1. **Static Generation** — All pages pre-rendered at build time (SSG)
2. **Client Interactions** — Contact form, blog/project/service detail pages
3. **Animations** — Framer Motion for scroll reveals, hover effects
4. **Routing** — Next.js App Router with nested dynamic routes
5. **State** — Component-local state + URL params for project filters

## [NEW_FEATURES]
1. **Interactive Brands** — Click-to-reveal info cards for each partner brand with product descriptions
2. **Services Comparison Table** — Responsive table showing installation/maintenance/repair for all 8 services
3. **Company Highlights** — 6 animated non-numeric highlights with scroll-reveal icons (Nationwide Coverage, Professional Engineering, Experienced Team, International Brands, Commercial Expertise, Lifecycle Service)
4. **Project Gallery** — Filterable project grid with fullscreen lightbox/modal, navigation arrows, and counter
5. **Before & After Slider** — Drag-to-compare comparison slider with 3 sample categories (Installation, AC Upgrade, Maintenance)
6. **Morocco Coverage Map** — SVG-based Morocco outline with 8 animated city markers (Casablanca, Rabat, Marrakech, Tangier, Agadir, Fes, Meknes, Oujda) with pulsing animations
7. **Floating Contact Widget** — Fixed bottom-right expandable widget with Phone, WhatsApp, Email buttons

## [ORPHANS & PENDING]
- [ ] User to upload official ECO AIR SERVICE logo (placeholder "EA" used)
- [ ] User to verify HVAC photos from Unsplash (can be replaced with local images)
- [ ] InteractiveBrands replaces PartnerBrands on home page; PartnerBrands still used on /about
- [ ] Before/After images use gradient placeholders; replace with actual project photos when available
