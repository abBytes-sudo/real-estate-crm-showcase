# Rent A Roof — Real-Estate CRM & Operations Platform

A production platform that runs a live real-estate brokerage end to end — **CRM, property inventory, automatic property↔lead matching, a public website + CMS, an AI front-desk assistant, a customer account area, and full analytics** — in one system.

> 🔒 **This is a public showcase.** The complete source lives in a **private** repository — I'm happy to grant access to serious reviewers on request. Every screenshot below uses **demo data** (real customer data, credentials, and phone numbers removed); the brand is shown as it runs in production.

---

## What it does

### 🎯 CRM & lead lifecycle
A complete lead pipeline: enquiries move through stages (New → Qualified → Property-matching → Visiting → Negotiating → Won/Lost), each with tasks, follow-ups, calling queues and role-based ownership. Every number on the dashboard opens the exact list behind it.

### 🏢 Inventory & multi-unit management
Full property inventory — residential & commercial, rent & sale, whole buildings with per-floor units, owner profiles, verification tiers and locality mastering. Composable status tiles double as filters, and a stacking-plan view manages every floor of a building as its own rentable unit.

### 🔗 Smart property ↔ lead matching
A suggestion engine automatically matches live inventory to open requirements — scoring each on BHK, area and budget — and raises **match alerts** when a new property fits a waiting lead, surfaced on the dashboard, the workspace and via notifications.

### 💬 Communications — the "front desk"
A unified inbox powered by **Roofie**, an AI assistant that greets website visitors, qualifies them and books visits, with a human able to step in anytime. Channels include WhatsApp, SMS and Email, with live KPIs.

### 🌐 Website, CMS & customer accounts
The public property website is part of the same platform: searchable listings from live inventory, locality guides, property-detail pages, a compare tray, and a phone-OTP **customer dashboard** (shortlist, enquiries, booked visits, saved searches). A full CMS drives pages, menus, blog and testimonials.

### 📊 Analytics & engagement tracking
Visitor tracking, campaign funnels (visitors → signups → enquiries → qualified → won → revenue), source attribution and per-property engagement — so every lead's journey is visible end to end.

---

## 📸 Screenshots

### 🌐 The public website
**Home** — hero search over live inventory
![Website home](screenshots/d01-website-home.png)

**Listings** — live inventory with the on-site assistant
![Website listings](screenshots/d02-website-listings.png)

**Property detail** — full spec sheet, gallery, similar listings and enquiry CTA
![Property detail](screenshots/d03-website-property-detail.png)

**Locality guides** — browse by neighbourhood
![Localities](screenshots/d04-website-localities.png)

### 👤 The customer account area (phone-OTP dashboard)
**Overview** — saved properties, open enquiries, next visit, new matches
![Customer dashboard](screenshots/d05-customer-dashboard.png)

**Shortlist** — everything the customer saved, in one place
![Customer shortlist](screenshots/d05b-customer-shortlist.png)

**Enquiries** — every enquiry they raised and where it stands with the desk
![Customer enquiries](screenshots/d05c-customer-enquiries.png)

**Visits** — booked site visits
![Customer visits](screenshots/d05d-customer-visits.png)

### 🎯 CRM — command centre
**Dashboard** — cohort board where every number opens its list
![CRM dashboard](screenshots/d06-crm-dashboard.png)

**Enquiries** — the full lead list with filters, smart views and match counts
![CRM enquiries](screenshots/d07-crm-enquiries.png)

### 🧭 The enquiry workspace
**Tasks & follow-ups** — the qualified lead, its requirement brief, and everything scheduled
![Enquiry workspace](screenshots/d08-crm-enquiry-workspace.png)

**Property suggestions** — live inventory matched to this requirement, best fit first
![Property suggestions](screenshots/d08b-crm-property-suggestions.png)

**Buckets** — curate a handpicked set and track it through Shared → Visited → Shortlisted → Finalised
![Buckets](screenshots/d08c-crm-buckets.png)

**Engagement** — what the customer actually did on the website (saved, viewed, searched)
![Enquiry engagement](screenshots/d08d-crm-enquiry-engagement.png)

**Shareable link** — a public, handpicked shortlist the customer opens with no login
![Shareable handpicked link](screenshots/d23-shareable-link.png)

### 🏢 Inventory & the property workspace
**Inventory** — live listings with photos, composable status facets and matching
![Inventory](screenshots/d11-crm-inventory.png)

**Property workspace — engagement** — website interest, owner panel and record for one listing
![Property workspace](screenshots/d12-crm-property-workspace.png)

**Suggested leads** — open requirements this property would suit, scored on fit
![Suggested leads](screenshots/d12b-crm-suggested-leads.png)

**Units & listings** — the building's stacking plan; each floor a separately rentable unit
![Units and listings](screenshots/d12c-crm-property-units.png)

**Property tasks** — visits and follow-ups scheduled against the listing
![Property tasks](screenshots/d12d-crm-property-tasks.png)

**Add a listing** — the guided intake with the per-location code matrix
![Add listing](screenshots/d13-crm-add-listing.png)

### ⚙️ Masters & configuration
**Localities master** ![Localities master](screenshots/d14-crm-localities-master.png)

**Pricing master** — requirement score = brief × market fit ![Pricing master](screenshots/d15-crm-pricing-master.png)

**Owner profiles** ![Owner profiles](screenshots/d16-crm-owner-profiles.png)

**Inventory activity** ![Inventory activity](screenshots/d17-crm-inventory-activity.png)

### 💬 Communications
**Roofie** — the AI front-desk inbox ![Roofie](screenshots/d10-crm-roofie-bot.png)

**Calling queues** — who to call next, in order ![Calling queues](screenshots/d09-crm-calling-queues.png)

### 📊 Analytics
**Campaign analytics** — UTM-scoped funnel from visitor to revenue
![Campaign analytics](screenshots/d18-crm-campaign-analytics.png)

**Website analytics** — traffic, property demand and visitor journeys
![Website analytics](screenshots/d19-crm-website-analytics.png)

**Activity manager** ![Activity manager](screenshots/d20-crm-activity.png)

### 👥 Team & operations
**Team & access** — roles, permissions and per-user controls ![Team](screenshots/d21-crm-team.png)

**Bulk actions** — select and act on many listings at once ![Bulk actions](screenshots/d22-crm-bulk-actions.png)

### 📱 Mobile
The CRM and website are built mobile-first — the mobile web app is a distinct, touch-native design, not a shrunk desktop.

| Website | Property | Customer dashboard |
|---|---|---|
| ![m home](screenshots/m01-website-home.png) | ![m property](screenshots/m02-website-property.png) | ![m dashboard](screenshots/m09-customer-dashboard.png) |

| CRM dashboard | Enquiries | Enquiry workspace |
|---|---|---|
| ![m crm dash](screenshots/m03-crm-dashboard.png) | ![m enquiries](screenshots/m04-crm-enquiries.png) | ![m workspace](screenshots/m05-crm-workspace.png) |

| Inventory | Property workspace | Roofie |
|---|---|---|
| ![m inventory](screenshots/m06-crm-inventory.png) | ![m property ws](screenshots/m08-crm-property-workspace.png) | ![m roofie](screenshots/m07-crm-roofie.png) |

---

## 🧰 Tech
`Laravel` · `Livewire` · `Alpine.js` · `Tailwind CSS` · `MySQL` · `PHP 8` · `Spatie Media Library` · REST APIs · web-push notifications

## 🔑 Want to see the code?
The complete source is in a **private repository**. I grant reviewer access on request — just reach out.

---
Built by **[@abBytes-sudo](https://github.com/abBytes-sudo)** · abhimasih0505@gmail.com · +91 73039 37702
