# 🎯 Project Brief — Entertainment Artist Website
**Prepared by:** Danny (Web Design)
**Date:** September 9, 2026
**Status:** Draft — Pending Client Review

---

## 👤 Client Overview

- **Name:** YSG Migo
- **Business:** Migo World Entertainment LLC
- **Industry:** Entertainment — Rapper / Event Promoter / Community Events
- **Location:** San Antonio, TX / McAllen, TX area
- **Notable Work:**
  - Event promoter
  - Youth Basketball Camp w/ San Antonio Spurs player
  - Active rapper / recording artist
- **Current Setup:** JotForm + Square (wants to replace/upgrade)
- **Goal:** One central website that handles everything — bookings, portfolio, merch, music, events, and payments

---

## 🎯 Project Goal

Build a **professional, all-in-one entertainment website** that:

1. Acts as his **digital headquarters** — everything lives here
2. Replaces the patchwork of JotForm + Square with a cleaner, cheaper system
3. Makes it easy for **fans** to find his music, buy merch, and RSVP to events
4. Makes it easy for **promoters and venues** to book him
5. Gives him **livestreaming capability** for virtual events and shows
6. Is **legally protected** (terms, privacy, waivers for youth events)
7. Is **secure** against hacks, fraud, and data breaches

---

## 📋 What We're Building — Full Feature List

### Pages (7 Core)

| Page | Purpose |
|---|---|
| **Home** | First impression — who he is, what he does, what to do next |
| **Music** | All music in one place — streaming embeds + free access |
| **Events** | Upcoming shows, past events, tickets, VIP, RSVP |
| **Store** | Merch — shirts, hats, limited drops, bundles |
| **Bookings / EPK** | Professional booking page for venues and promoters |
| **About** | His story, community work, career highlights |
| **Contact** | Separated inboxes for booking, press, merch, general |

### Key Features

**Music**
- Embedded Spotify + Apple Music players
- YouTube music video section
- SoundCloud (freestyles / unreleased)
- Smart link (one link routes fans to their preferred platform)
- Optional free download (email capture)

**Events & Ticketing**
- Upcoming event calendar
- Individual event landing pages (like the basketball camp — full page with flyer, details, form, checkout)
- Ticket sales directly through the website (no JotForm middleman)
- Digital registration + waiver for youth events
- VIP / table reservations
- Past events gallery (photos, recaps)
- RSVP + waitlist

**Store / Merch**
- Clean product grid
- Print-on-demand (Printful) — no inventory needed
- Ticket + merch bundles
- Discount codes
- Mobile-optimized checkout
- Order tracking

**Bookings**
- Professional EPK (Electronic Press Kit) page
- Downloadable EPK PDF
- High-res press photo downloads
- Booking inquiry form (date, venue, event type, attendance, budget, performance length)

**Livestreaming**
- Embedded YouTube Live or Twitch directly on the website
- Fans watch on HIS site, not YouTube's homepage
- Future option: paid livestream tickets via Stripe

**Fan Engagement**
- Email list signup (front and center)
- SMS signup (optional)
- All social media links
- Fan club / membership (Phase 2)

---

## 💳 Payment Processing — Replacing Square

### The Problem with Square
Square charges **2.9% + $0.30 per online transaction**.
On the basketball camp alone ($40,000 gross), Square took approximately **$1,200+ in fees**.

### The Solution — Stripe (Online) + Helcim (In-Person)

| Use Case | Processor | Fee Structure |
|---|---|---|
| **Website checkout** (merch, tickets, event registration) | **Stripe** | 2.9% + $0.30 flat |
| **In-person events** (on-site POS, card reader) | **Helcim** | Interchange + 0.25% + $0.08 |

### Why This Combo?

**Stripe for online:**
- Integrates directly and cleanly into Framer (website builder)
- Handles merch, tickets, registrations, and livestream access in one place
- Built-in fraud protection (Stripe Radar)
- Industry standard — most reliable for website e-commerce
- $0/month

**Helcim for in-person:**
- Interchange-plus pricing = dramatically cheaper than Square's flat rate
- No monthly fee
- On a $40K in-person event: Helcim ~$800 vs Square ~$1,200 = **$400 saved per event**
- Hardware: ~$99-119 terminal (one-time cost)

### Real Fee Comparison (Online Transactions)

| Transaction | Card Type | Stripe | Helcim | Savings |
|---|---|---|---|---|
| $10 merch | Premium rewards | $0.59 | $0.54 | $0.05 |
| $50 ticket | Standard credit | $1.75 | $1.30 | $0.45 |
| $160 youth camp | Standard credit | $4.94 | $3.61 | **$1.33** |
| $160 youth camp | Debit | $4.94 | $1.85 | **$3.09** |

> **Note:** Stripe is used for online checkout because it integrates natively with Framer. Helcim's online integration requires more custom development. For a future upgrade, Helcim online can replace Stripe entirely and save even more.

**Total monthly processing cost: $0** (pay per transaction only)

---

## 🔒 Legal Protection

### Required Legal Pages
1. Terms of Service — refunds, cancellations, merch returns
2. Privacy Policy — required by law (collecting emails + payments)
3. Refund Policy — events (no refund) vs merch (exchanges)
4. Cookie Policy

### Youth Event Protection
- Digital liability waiver — parents/guardians sign before checkout
- Photo/video release consent
- Emergency contact collection
- Age verification (confirming registrant is parent/guardian)

### General Security
- SSL certificate (HTTPS) — Stripe requires it
- Custom domain email (ex: `booking@migoworldent.com`)
- 2FA on all accounts (domain, hosting, Stripe, Helcim, social)
- CAPTCHA on all public forms
- Weekly automated backups

---

## 🛠️ Tech Stack

| Function | Tool | Cost |
|---|---|---|
| Website | **Framer Pro** | ~$25/mo (billed to client) |
| Online payments | **Stripe** | 2.9% + $0.30/transaction |
| In-person payments | **Helcim** | Interchange + 0.25% + $0.08 |
| Merch fulfillment | **Printful** | Per order, no monthly fee |
| Music smart link | **Linkfire** or **Feature.fm** | Free tier |
| Livestreaming | **YouTube Live** (embedded) | Free |
| Email marketing | **Mailchimp** | Free up to 500 contacts |
| Forms + waivers | **Tally.so** | Free |
| Domain | **Namecheap** (`migoworldent.com`) | ~$10/year |
| Email routing | **Cloudflare** | Free |
| Analytics | **Google Analytics** | Free |

**Client's monthly cost: ~$25/mo (Framer Pro) + processing fees per transaction**

---

## 📅 Timeline

| Phase | What | When |
|---|---|---|
| 1 | Client info gathering (bio, photos, music links, brand colors) | Day 1 |
| 2 | Site design + structure — client reviews | Days 2–4 |
| 3 | Payment setup (Stripe + Helcim accounts, test checkout) | Days 4–5 |
| 4 | Content population (music, events, merch, photos) | Days 5–7 |
| 5 | Legal pages + security setup | Days 7–9 |
| 6 | Testing + launch | Days 9–10 |
| 7 | Post-launch support + tweaks | Ongoing |

**Estimated launch: 4 days to 2 weeks from project start**

---

## 📥 What We Need From You (YSG Migo)

### Branding
- [ ] Confirm domain: `migoworldent.com`
- [ ] Brand colors (or leave to designer)
- [ ] Logo (existing or direction for new one)
- [ ] Professional photos (high-res, multiple)

### Music
- [ ] Spotify artist link
- [ ] Apple Music link
- [ ] YouTube channel link
- [ ] SoundCloud link (if applicable)
- [ ] Any other platforms (Audiomack, Tidal, etc.)
- [ ] Which release to feature first

### Events
- [ ] Upcoming events (dates, venues)
- [ ] Past event photos (for gallery)
- [ ] Event flyers
- [ ] Basketball camp details + photos

### Store
- [ ] Merch items (products, sizes, colors)
- [ ] Existing merch photos
- [ ] Pricing

### Bookings
- [ ] Short bio + long bio
- [ ] Performance types offered
- [ ] Cities/regions available
- [ ] Booking contact email

### Social Media Handles
- [ ] Instagram: @
- [ ] TikTok: @
- [ ] Twitter/X: @
- [ ] Facebook:
- [ ] YouTube:
- [ ] Spotify:
- [ ] Snapchat: @

---

## 💰 Compensation

- **Payment:** 2% of gross revenue — ongoing
- **Applies to:** All revenue generated through or promoted via the website
- **Formal agreement:** Separate Revenue Share Agreement (signed by both parties)

---

*Prepared by Danny | September 9, 2026*
