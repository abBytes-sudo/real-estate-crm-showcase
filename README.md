# Rent A Roof — Real-Estate CRM & Operations Platform

I built this for **Rent A Roof**, a live real-estate brokerage in South Delhi, as a one-man team — design, build and deploy — driven end to end through agentic AI workflows. It started as a way to stop losing leads in spreadsheets and grew into the system the whole company runs on: CRM, property inventory, automatic property↔lead matching, the public website and its CMS, an AI front-desk assistant, deals & closures, and the reporting behind all of it. One system, one login, one source of truth. It's in production today at rentaroof.in.

Everything below is real, working software. The CRM screenshots use demo data — I stripped out the real customers, numbers and keys before publishing — and the public-website shots are from the live site.

*The full source is in a private repo; I'm glad to walk a serious reviewer through it on request.*

---

## What it does

**CRM & lead lifecycle.** Enquiries move New → Qualified → Property-matching → Visiting → Negotiating → Won/Lost, each with tasks, follow-ups, calling queues and role-based ownership. Every number on the dashboard opens the exact list behind it.

**Inventory & multi-unit management.** Residential and commercial, rent and sale, whole buildings broken into per-floor units, owner profiles, verification tiers, locality mastering. The status tiles double as composable filters, and a stacking-plan view treats every floor as its own rentable unit.

**Smart property ↔ lead matching.** A suggestion engine scores live inventory against open requirements (BHK, area, budget) and raises match alerts when a new property fits a waiting lead.

**Deals & closures.** A booked-deal pipeline with token and payment tracking, commission, agreement generation and closure states — plus win-rate and conversion KPIs.

**The front desk.** A unified inbox powered by Roofie, an assistant that greets website visitors, reads a free-text brief, pulls live matches, quotes neighbourhood price bands and books visits — with a human able to step in anytime.

**Website, CMS & customer accounts.** The public property site is part of the same platform: searchable listings, locality guides, a compare tray, a phone-OTP customer dashboard, and a full CMS for pages, menus, blog and testimonials.

**Analytics.** Visitor tracking, campaign funnels (visitors → signups → enquiries → qualified → won → revenue), source attribution and per-property engagement.

---

## Screenshots

### The public website *(live production)*
**Home** — hero search over live inventory
![Website home](screenshots/d01-website-home.jpg)

**Listings** — live inventory with the on-site assistant
![Website listings](screenshots/d02-website-listings.jpg)

**Property detail** — full spec sheet, gallery, similar listings and enquiry CTA
![Property detail](screenshots/d03-website-property-detail.jpg)

**Locality guides** — every serviced colony, written up by the team
![Locality guides](screenshots/d04-website-localities.jpg)

**Locality detail** — the area in the team's words: getting around, price bands, live listings
![Locality detail](screenshots/d04b-website-locality-detail.jpg)

### The customer account area (phone-OTP dashboard)
**Overview** — saved properties, open enquiries, next visit, new matches
![Customer dashboard](screenshots/d05-customer-dashboard.png)

**Shortlist** ![Shortlist](screenshots/d05b-customer-shortlist.png)
**Enquiries** ![Customer enquiries](screenshots/d05c-customer-enquiries.png)
**Visits** ![Customer visits](screenshots/d05d-customer-visits.png)

### CRM — command centre
**Dashboard** — a cohort board where every number opens its list
![CRM dashboard](screenshots/d06-crm-dashboard.png)

**Enquiries** — the full lead list with smart views, filters and match counts
![CRM enquiries](screenshots/d07-crm-enquiries.png)

### The enquiry workspace
**Tasks & follow-ups** — the qualified lead, its requirement brief, everything scheduled
![Enquiry workspace](screenshots/d08-crm-enquiry-workspace.png)

**Property suggestions** — live inventory matched to the requirement, best fit first
![Property suggestions](screenshots/d08b-crm-property-suggestions.png)

**Buckets** — curate a handpicked set, track it Shared → Visited → Shortlisted → Finalised
![Buckets](screenshots/d08c-crm-buckets.png)

**Engagement** — what the customer actually did on the website (saved, viewed, searched)
![Enquiry engagement](screenshots/d08d-crm-enquiry-engagement.png)

**Shareable link** — a public, handpicked shortlist the customer opens with no login
![Shareable handpicked link](screenshots/d23-shareable-link.png)

### Inventory & the property workspace
**Inventory** — live listings with photos, composable status facets and matching
![Inventory](screenshots/d11-crm-inventory.png)

**Property workspace — engagement** ![Property workspace](screenshots/d12-crm-property-workspace.png)
**Suggested leads** — open requirements this property suits, scored on fit ![Suggested leads](screenshots/d12b-crm-suggested-leads.png)
**Units & listings** — the building's stacking plan; each floor a separate unit ![Units](screenshots/d12c-crm-property-units.png)
**Property tasks** ![Property tasks](screenshots/d12d-crm-property-tasks.png)
**Add a listing** — guided intake with the per-location code matrix ![Add listing](screenshots/d13-crm-add-listing.png)

### Deals & closures
**Pipeline** — booked deals by stage with win-rate, conversion and token KPIs
![Deals](screenshots/e05-deals.png)

**Deal workspace** — a closed-won deal: parties, pipeline, agreement, documents
![Deal workspace](screenshots/e06-deal-workspace.png)

### Tasks & follow-ups
Every call, visit and follow-up across the team, in one queue.
![Tasks](screenshots/e07-tasks.png)

### Website CMS
**Pages** — public pages built from editable section blocks ![CMS pages](screenshots/e01-cms-pages.png)
**Menus & footer** ![CMS menus](screenshots/e02-cms-menus.png)
**Blog & news** ![CMS blog](screenshots/e03-cms-blog.png)
**Testimonials** — video & written reviews, publish toggles ![CMS testimonials](screenshots/e04-cms-testimonials.png)

### Masters & configuration
**Localities master** ![Localities master](screenshots/d14-crm-localities-master.png)
**Pricing master** — requirement score = brief × market fit ![Pricing master](screenshots/d15-crm-pricing-master.png)
**Owner profiles** ![Owner profiles](screenshots/d16-crm-owner-profiles.png)
**Inventory activity** ![Inventory activity](screenshots/d17-crm-inventory-activity.png)
**Configurator** — the shared dropdown vocabulary behind every form ![Configurator](screenshots/e10-vocabularies.png)
**Preferences** ![Preferences](screenshots/e09-settings-preferences.png)

### Users, roles & permissions
**Team & access** ![Team](screenshots/d21-crm-team.png)
**Roles & permissions** ![Roles](screenshots/e08-roles-permissions.png)

### Import / export
**Enquiries import workbook** ![Enquiries import](screenshots/e11-enquiries-import.png)
**Inventory import workbook** ![Inventory import](screenshots/e12-inventory-import.png)

### Bulk actions
**Enquiries** — WhatsApp, SMS, Email, calling queue, assign, follow-up, level, flag, tag, export
![Enquiries bulk](screenshots/e15-enquiries-bulk.png)

**Inventory** — status, publish, feature, descriptions, reassign, message owners, verify, copy links, export, delete
![Inventory bulk](screenshots/e16-inventory-bulk.png)

### Communications & the Roofie assistant
**Calling queues** — who to call next, in priority order ![Calling queues](screenshots/d09-crm-calling-queues.png)
**Front-desk inbox (CRM)** — every bot conversation, with human takeover ![Roofie inbox](screenshots/d10-crm-roofie-bot.png)
**On the website** — greets, qualifies, offers quick actions ![Roofie assistant](screenshots/e18-roofie-assistant.png)
**Reads a free-text brief** — pulls live matches, quotes the area's price band, offers to save the search & book a visit ![Roofie conversation](screenshots/e18b-roofie-conversation.png)

### Analytics
**Campaign analytics** — a UTM funnel from visitor to revenue ![Campaign analytics](screenshots/d18-crm-campaign-analytics.png)
**Website analytics** — traffic, property demand, visitor journeys ![Website analytics](screenshots/d19-crm-website-analytics.png)
**Activity manager** ![Activity manager](screenshots/d20-crm-activity.png)

### Collapsible navigation
One accordion sidebar that collapses to an icon rail (⌘B) — more room for the work.
![Collapsed sidebar](screenshots/e17-sidebar-collapsed.png)

---

## Mobile
The CRM and the website are mobile-first — the mobile web app is a distinct, touch-native design, not a shrunk desktop.

**Website & customer**
| Home | Property | Locality guides | Locality detail | Customer dashboard |
|---|---|---|---|---|
| ![](screenshots/m01-website-home.jpg) | ![](screenshots/m02-website-property.jpg) | ![](screenshots/m28-website-localities.jpg) | ![](screenshots/m29-website-locality-detail.jpg) | ![](screenshots/m09-customer-dashboard.png) |

**CRM core**
| Dashboard | Enquiries | Enquiry workspace | Inventory | Property workspace |
|---|---|---|---|---|
| ![](screenshots/m03-crm-dashboard.png) | ![](screenshots/m04-crm-enquiries.png) | ![](screenshots/m05-crm-workspace.png) | ![](screenshots/m06-crm-inventory.png) | ![](screenshots/m08-crm-property-workspace.png) |

**Deals, tasks & bulk**
| Deals | Deal workspace | Tasks | Enquiries bulk | Inventory bulk |
|---|---|---|---|---|
| ![](screenshots/m14-deals.png) | ![](screenshots/m15-deal-workspace.png) | ![](screenshots/m16-tasks.png) | ![](screenshots/m24-enquiries-bulk.png) | ![](screenshots/m25-inventory-bulk.png) |

**CMS, config & analytics**
| CMS pages | Menus | Blog | Testimonials | Configurator |
|---|---|---|---|---|
| ![](screenshots/m10-cms-pages.png) | ![](screenshots/m11-cms-menus.png) | ![](screenshots/m12-cms-blog.png) | ![](screenshots/m13-cms-testimonials.png) | ![](screenshots/m19-vocabularies.png) |

| Roles & permissions | Preferences | Enquiries import | Inventory import | Campaign analytics |
|---|---|---|---|---|
| ![](screenshots/m17-roles-permissions.png) | ![](screenshots/m18-settings.png) | ![](screenshots/m20-enquiries-import.png) | ![](screenshots/m21-inventory-import.png) | ![](screenshots/m22-campaign-analytics.png) |

**Website analytics, drawer & Roofie**
| Website analytics | Collapsible drawer | Roofie assistant |
|---|---|---|
| ![](screenshots/m23-website-analytics.png) | ![](screenshots/m26-drawer-menu.png) | ![](screenshots/m27-roofie.png) |

---

## How I built it
Solo, end to end, using agentic AI workflows — I ran the requirements and the product decisions, then directed AI coding agents through the architecture, the implementation and the deployments, reviewing and steering at every step. It's the same way I work across all of these projects.

## Tech
Laravel · Livewire · Alpine.js · Tailwind CSS · MySQL · PHP 8 · Spatie Media Library · REST APIs · web-push notifications

---
Developed by **[@abBytes-sudo](https://github.com/abBytes-sudo)** for Rent A Roof · abhimasih0505@gmail.com · +91 73039 37702
