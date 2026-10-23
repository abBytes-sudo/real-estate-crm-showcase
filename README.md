# Real Estate Platform — CRM & operations

**Status:** live since the 9 Sep 2026 cutover ([Live site](https://rentaroof.in)); in daily use by the Rent A Roof team.
**My role:** Operations & CRM Lead. Requirements, AI-assisted build (I direct AI coding agents; I don't hand-code), data migration, testing, go-live and team training.
**▶ [Interactive demo](https://abbytes-sudo.github.io/real-estate-crm-showcase/)** · source in a private repo; walkthrough on request.

Rent A Roof, a South Delhi property-consultation company, ran sales on Buildesk, a 12-seat subscription CRM (about ₹1.44 lakh a year). Between June and September 2026 I led its move to a self-hosted CRM with an integrated public website: lead pipeline, a 12,152-listing inventory (22 Oct 2026) kept current by Excel and magazine-PDF importers, nightly property↔lead matching, tasks and reminders, deals, a website CMS and analytics.

**Results** (production data from read-only queries, 22–23 Oct 2026)
- **Organic leads, first 1.5 months after go-live (9 Sep – 23 Oct 2026):** 113 of 383 new leads came in organically, not from paid ads or portals: 45 Instagram DMs, 27 website and Roofie leads, 25 inbound phone calls, 15 WhatsApp messages and 1 broker referral. Instagram and WhatsApp leads are messages the team logged in the CRM; of the 27 website leads, 9 came from Google search. 58 of the 113 organic leads (51%) now have a qualified requirement, against 57 of 258 Meta-ad leads (22%).
- **Organic property enquiries, same window:** 16 new leads enquired organically about a specific listing, all through Roofie on the listing page; 8 of them arrived from Google search. Organic Google visitors grew from 14 to 369 a week within a month of the Sep 2026 relaunch.
- 6,089 legacy lead records and 27,516 history events migrated in one import, 0 rejected (30 Jul 2026).
- 2,248 property↔lead matches and 2,397 completed tasks in the 30 days to 22 Oct 2026, up from 1,887 matches and 1,014 tasks in the 30 days to 5 Oct.
- The monthly listings magazine loads by PDF upload: the Sept 2026 issue had 10,639 lines read and 99.3% classified automatically; the October issue was applied on 13 Oct 2026.

Screenshots are from a demo build: placeholder brand, fictional people and demo figures (the only production numbers are the dated ones in this write-up), with phone numbers, house numbers and owner names masked. Layouts and flows match production. "abBytes" in the screenshots is the demo build's placeholder brand, not a real company.

---

## October 2026 — what's new since go-live

What went live or grew after the 9 Sep cutover, with what production shows as of 22 Oct 2026:

- **Listing verification desk ("Survey master", from 9–11 Oct) and owner-calling screen (live 21 Oct).** One desk to keep listings verified, plus a guided screen for calling owners and logging each result. 815 listing-check tasks created, 789 done; 148 owner calls logged in the calling screen's first 2 days (3 callers, 71 owners); 1,644 listings verified to date, up from 1,099 on 5 Oct.
- **Tasks & follow-ups redesign (Oct 2026).** Board and calendar views, quick filters and a reschedule-overdue dialog. 2,397 tasks completed in the 30 days to 22 Oct (1,608 client work + 789 listing checks), up from 1,014 in the 30 days to 5 Oct. Client-work tasks went from 121–199 a week in September to 334–505 a week in October.
- **Property↔lead matching.** 2,248 matches in the 30 days to 22 Oct, covering 141 requirements and 827 listings, up from 1,887 on 5 Oct.
- **October magazine import (applied 13 Oct).** 9,186 lines recognised; 1,178 listings updated, 552 created, 88 reactivated and 594 retired.
- **Inventory data quality.** A builders directory (224 firms, 324 phone numbers linked, 54 duplicate spellings merged); data-quality flags (1,461 raised since 4 Oct, 177 resolved); and a free-text staff property search, where "3 BHK GK1 2nd floor" becomes filters (1,463 searches by 8 staff since 6 Oct).
- **Ad-campaign tags.** 261 enquiries carry an ad-campaign (UTM) tag, up from near zero before October.
- **Deals.** The first 2 deals recorded as won in the CRM (Oct 2026); brokerage dues tracked (2 paid, 3 payments recorded).

*Built, not yet in use (as of 22 Oct 2026):* SMS campaigns and automations, deal approvals, and field-trip planning (0 campaigns sent, 0 approval requests, 0 trips or visit requests).

---

## What it does

**CRM & lead lifecycle.** Enquiries move New → Qualified → Property-matching → Visiting → Negotiating → Won/Lost, each with tasks, follow-ups, calling queues and role-based ownership. Every number on the dashboard opens the exact list behind it. Click-to-call runs through Knowlarity cloud telephony and SMS through DLT-registered templates, both set up by me.

**Inventory & multi-unit management.** Residential and commercial, rent and sale, whole buildings broken into per-floor units, owner profiles, verification tiers, locality mastering. The status tiles double as composable filters, and a stacking-plan view treats every floor as its own rentable unit.

**Property ↔ lead matching.** A nightly suggestion engine scores live inventory against open requirements (BHK, area, budget) and raises match alerts when a new property fits a waiting lead.

**Deals & closures.** A booked-deal pipeline with token and payment tracking, commission and brokerage dues, agreement generation and closure states, plus win-rate and conversion KPIs.

**The front desk.** A unified inbox for Roofie, a scripted (rule-based) enquiry assistant, not AI. It greets website visitors, reads a free-text brief, pulls live matches, quotes neighbourhood price bands and offers to book a visit, and a person can step in anytime. From 7 Sep to 23 Oct 2026, 78 of 87 website chats (90%) never needed an agent, and 28 became or joined an enquiry.

**Website, CMS & customer accounts.** The public property site is part of the same platform: 6,843 active listings published straight from CRM inventory (22 Oct 2026), searchable listings, locality guides, a compare tray, a phone-OTP customer dashboard, and a CMS for pages, menus, blog, FAQ and testimonials.

**Analytics.** Visitor tracking, campaign funnels for UTM-tagged traffic (visitors → signups → enquiries → qualified → deals won), source attribution and per-property engagement.

---

## Screenshots

### The public website *(demo build; live at rentaroof.in)*
**Search & listings** — plain-English search over live inventory, with Roofie docked alongside
![Website listings page with search bar, property cards and the Roofie panel](screenshots/d02-website-listings.jpg)

**Property detail** — full spec sheet, gallery, verification status, other units in the building, what's nearby and the enquiry CTA
![Property detail page](screenshots/d03-website-property-detail.jpg)

**Locality guides** — every serviced colony, written up by the team (top of the index page)
![Locality guides index](screenshots/d04-website-localities.jpg)

**Locality detail** — the area in the team's words: getting around, price bands, live listings
![Locality detail page for one colony](screenshots/d04b-website-locality-detail.jpg)

**Compare** — put up to four listings side by side
![Compare page with two listings side by side](screenshots/e23-website-compare.jpg)

### The customer account area (phone-OTP dashboard)
**Overview** — saved properties, open enquiries, next visit, new matches
![Customer dashboard overview](screenshots/d05-customer-dashboard.png)

**Shortlist** ![Customer shortlist](screenshots/d05b-customer-shortlist.png)
**Enquiries** ![Customer enquiries](screenshots/d05c-customer-enquiries.png)
**Visits** ![Customer visits](screenshots/d05d-customer-visits.png)

### CRM — command centre
**Dashboard** — a cohort board where every number opens its list
![CRM dashboard with today's brief and stage tiles](screenshots/d06-crm-dashboard.png)

**Enquiries** — the full lead list with smart views, filters and match counts
![CRM enquiries list](screenshots/d07-crm-enquiries.png)

### The enquiry workspace
**Tasks & follow-ups** — everything scheduled on a qualified lead, with internal team notes alongside
![Enquiry workspace on the Tasks tab](screenshots/d08-crm-enquiry-workspace.png)

**Buckets** — curate a handpicked set, track it Shared → Visited → Shortlisted → Finalised
![Enquiry buckets tab](screenshots/d08c-crm-buckets.png)

**Engagement** — what the customer actually did on the website (saved, viewed, searched)
![Enquiry engagement tab](screenshots/d08d-crm-enquiry-engagement.png)

**Shareable link** — a public, handpicked shortlist the customer opens with no login
![Shareable handpicked shortlist page](screenshots/d23-shareable-link.png)

### Inventory & the property workspace
**Inventory** — live listings with photos, composable status facets and matching
![Inventory list with status tiles](screenshots/d11-crm-inventory.png)

**Property workspace** — engagement on one listing, with suggested leads (matching in reverse), units & listings and tasks one tab away
![Property workspace on the Engagement tab](screenshots/d12-crm-property-workspace.png)

**Add a listing** — guided intake with the per-location code matrix ![Add-listing form](screenshots/d13-crm-add-listing.png)

### Deals & closures
**Pipeline** — booked deals by stage with win-rate, conversion and token KPIs
![Deals pipeline](screenshots/e05-deals.png)

### Tasks & follow-ups
Every call, visit and follow-up across the team, in one queue.
![Tasks and follow-ups list](screenshots/e07-tasks.png)

### Website CMS
**Pages** — public pages built from editable section blocks ![CMS pages list](screenshots/e01-cms-pages.png)
**Menus & footer** ![CMS menus and footer editor](screenshots/e02-cms-menus.png)
**Blog & news** ![CMS blog and news list](screenshots/e03-cms-blog.png)
**FAQ** ![FAQ CMS](screenshots/e20-faq-cms.png)

### Masters & configuration
**Localities master** ![Localities master](screenshots/d14-crm-localities-master.png)
**Pricing master** — requirement score = brief × market fit ![Pricing master](screenshots/d15-crm-pricing-master.png)
**Inventory activity** ![Inventory activity by person](screenshots/d17-crm-inventory-activity.png)
**Configurator** — the shared dropdown vocabulary behind every form ![Configurator](screenshots/e10-vocabularies.png)
**Amenities master** — the shared amenities catalogue behind the forms, filters, import/export and website tiles ![Amenities master](screenshots/e19-amenities-master.png)
**Preferences** ![Notification preferences](screenshots/e09-settings-preferences.png)

### Users, roles & permissions
**Team & access** ![Team and access list](screenshots/d21-crm-team.png)
**Roles & permissions** ![Roles and permissions matrix](screenshots/e08-roles-permissions.png)

### Import / export
**Enquiries import workbook** ![Enquiries import](screenshots/e11-enquiries-import.png)
**Inventory import workbook** ![Inventory import](screenshots/e12-inventory-import.png)

### Bulk actions
**Enquiries** — WhatsApp (click-to-chat), SMS, email, calling queue, assign, follow-up, level, flag, tag, export
![Enquiries list with the bulk-action bar](screenshots/e15-enquiries-bulk.png)

**Inventory** — status, publish, feature, descriptions, reassign, message owners, verify, copy links, export, delete
![Inventory list with the bulk-action bar](screenshots/d22-crm-bulk-actions.png)

### Communications & the Roofie assistant
**Calling queues** — who to call next, in priority order ![Calling queues](screenshots/d09-crm-calling-queues.png)
**Front-desk inbox (CRM)** — every Roofie conversation, with human takeover ![Roofie inbox in the CRM](screenshots/d10-crm-roofie-bot.png)
**On the website** — Roofie (scripted, rule-based) greets, qualifies and offers quick actions ![Roofie quick actions on the website](screenshots/e18-roofie-assistant.jpg)
**Reads a free-text brief** — rule-based replies that pull live matches, quote the area's price band, and offer to save the search and book a visit ![Roofie conversation](screenshots/e18b-roofie-conversation.png)

### Analytics
**Campaign analytics** — a UTM funnel from visitor to deal won, for UTM-tagged traffic ![Campaign analytics](screenshots/d18-crm-campaign-analytics.png)
**Website analytics** — traffic, property demand, visitor journeys ![Website analytics](screenshots/d19-crm-website-analytics.png)
**Activity manager** ![Activity manager](screenshots/d20-crm-activity.png)

### Collapsible navigation
One accordion sidebar that collapses to an icon rail (⌘B) — more room for the work.
![Dashboard with the sidebar collapsed to an icon rail](screenshots/e17-sidebar-collapsed.png)

### Supply
**List-your-property** — the owner-supply triage desk (submissions from the website → verify → list). In production, 8 owners submitted a property between 20 Sep and 23 Oct 2026, and the team has marked 4 of them as listed.
![List-your-property triage desk](screenshots/e22-list-your-property.png)

---

## Mobile
The CRM and the website are mobile-first — the mobile web app is a distinct, touch-native design, not a shrunk desktop.

**Website & customer**
| Property | Locality guides | Locality detail | Compare | Customer dashboard |
|---|---|---|---|---|
| ![Mobile: property page](screenshots/m02-website-property.jpg) | ![Mobile: locality guides](screenshots/m28-website-localities.jpg) | ![Mobile: locality detail](screenshots/m29-website-locality-detail.jpg) | ![Mobile: compare](screenshots/m34-website-compare.jpg) | ![Mobile: customer dashboard](screenshots/m09-customer-dashboard.png) |

**CRM core**
| Dashboard | Enquiries | Enquiry workspace | Inventory | Roofie inbox |
|---|---|---|---|---|
| ![Mobile: CRM dashboard](screenshots/m03-crm-dashboard.png) | ![Mobile: enquiries](screenshots/m04-crm-enquiries.png) | ![Mobile: enquiry workspace](screenshots/m05-crm-workspace.png) | ![Mobile: inventory](screenshots/m06-crm-inventory.png) | ![Mobile: Roofie inbox](screenshots/m07-crm-roofie.png) |

**Deals, tasks & bulk**
| Deals | Tasks | Enquiries bulk | Inventory bulk |
|---|---|---|---|
| ![Mobile: deals](screenshots/m14-deals.png) | ![Mobile: tasks](screenshots/m16-tasks.png) | ![Mobile: enquiries bulk actions](screenshots/m24-enquiries-bulk.png) | ![Mobile: inventory bulk actions](screenshots/m25-inventory-bulk.png) |

**CMS & configuration**
| CMS pages | Menus | Blog | FAQ CMS | Configurator |
|---|---|---|---|---|
| ![Mobile: CMS pages](screenshots/m10-cms-pages.png) | ![Mobile: menus](screenshots/m11-cms-menus.png) | ![Mobile: blog](screenshots/m12-cms-blog.png) | ![Mobile: FAQ CMS](screenshots/m31-faq-cms.png) | ![Mobile: configurator](screenshots/m19-vocabularies.png) |

| Roles & permissions | Preferences | Enquiries import | Inventory import | Amenities master |
|---|---|---|---|---|
| ![Mobile: roles and permissions](screenshots/m17-roles-permissions.png) | ![Mobile: preferences](screenshots/m18-settings.png) | ![Mobile: enquiries import](screenshots/m20-enquiries-import.png) | ![Mobile: inventory import](screenshots/m21-inventory-import.png) | ![Mobile: amenities master](screenshots/m30-amenities-master.png) |

**Analytics, navigation & supply**
| Campaign analytics | Website analytics | Collapsible drawer | List-your-property |
|---|---|---|---|
| ![Mobile: campaign analytics](screenshots/m22-campaign-analytics.png) | ![Mobile: website analytics](screenshots/m23-website-analytics.png) | ![Mobile: navigation drawer](screenshots/m26-drawer-menu.png) | ![Mobile: list-your-property](screenshots/m33-list-your-property.png) |

---

## How I built it
AI-assisted delivery: I owned the requirements, data migration, testing, go-live and team training, and directed AI coding agents through the build. I don't hand-code. Earlier versions of the Rent A Roof website were built by outside teams that I coordinated.

## Tech
Laravel · Livewire · Alpine.js · Tailwind CSS · MySQL · PHP 8 · Spatie Media Library · REST APIs · web-push notifications · Knowlarity cloud telephony · DLT SMS

---
Developed by **[@abBytes-sudo](https://github.com/abBytes-sudo)** for Rent A Roof · [LinkedIn](https://www.linkedin.com/in/abhishek-m-b934a925a)

© 2026 Abhishek Anand Masih. Write-up and screenshots shared for portfolio review; not licensed for reuse.
