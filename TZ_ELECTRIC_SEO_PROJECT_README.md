# TZ Electric Inc. — SEO Overhaul Project

## Project Context Document

> **Purpose:** This document is a complete knowledge transfer file. Any AI assistant, developer, or team member reading this should be able to fully understand the current state of the TZ Electric SEO project, what was done, how it was done, what tools were used, and what remains. Attach this file to any AI conversation to resume work seamlessly.

---

## Quick Reference

| Field | Value |
|---|---|
| **Client** | TZ Electric Inc. |
| **Client Contact** | Tyler Zitz (Owner / Master Electrician) |
| **Agency** | CQ Marketing (Cesar — Founder) |
| **Website** | https://tzelectricinc.com |
| **Platform** | Webflow (CMS + Designer) |
| **Webflow Site ID** | `67ac70b9e25b6a62ed436918` |
| **Project Dates** | February 12–13, 2026 |
| **Status** | Phase 1 Complete — All changes live & published |
| **Report File** | `TZ_Electric_SEO_Report_FINAL.html` (interactive HTML report for Tyler) |

---

## Business Profile

TZ Electric Inc. is a Hudson Valley, NY–based contractor offering **both HVAC and electrical services**. This dual identity is central to the entire SEO strategy.

### Key Credentials
- **Mitsubishi Diamond Elite Contractor** — Highest-tier HVAC certification from Mitsubishi Electric. Major competitive differentiator. Previously mentioned only once on the entire site.
- **Generac Authorized Dealer** — Standby generator installation and service.
- **Master Electrician** — Tyler Zitz holds a Master Electrician license.
- **BBB A+ Accredited** — Since 2023.
- **5.0 stars / 200+ Google Reviews**

### Physical Location
```
TZ Electric Inc.
5079 Route 32
Catskill, NY 12414
Phone: (518) 678-1230
Hours: Mon–Fri 7:00 AM – 5:00 PM
```

### Service Area
- **Counties:** Greene, Dutchess, Ulster, Columbia
- **Cities:** Catskill, Hudson, Woodstock, Rhinebeck, Hunter, Kingston, Saugerties

### Services Offered
- Electrical: residential wiring, commercial wiring, indoor/outdoor electrical, service upgrades, electrification, EV charger installation
- HVAC: mini split installation (Mitsubishi), ductless heat pumps, central HVAC
- Generators: Generac standby generators, emergency power
- Hot Water Heaters: electric, hybrid, on-demand

---

## Core SEO Strategy

### The "50/50 Rebalance"

The site was previously positioned ~80% as an electrical contractor despite TZ Electric's significant HVAC business and Diamond Elite certification. The overhaul rebalanced the entire site to a **50/50 HVAC and electrical split**.

**What this means in practice:**
- Every page title, meta description, and OG tag was rewritten to include both HVAC and electrical keywords
- "Mitsubishi Diamond Elite" now appears across mini split, HVAC, home, financing, and career pages
- "Generac Authorized Dealer" features on generator and electrical pages
- Location pages target both service verticals for each geographic area

### Target Keyword Clusters

**HVAC Side:**
- Mitsubishi Diamond Elite Contractor
- Mini Split Installation [city/county]
- Ductless Heat Pumps Hudson Valley
- Heat Pump Installer Catskill NY
- HVAC Services Greene County

**Electrical Side:**
- Generac Authorized Dealer Hudson Valley
- Licensed Electrician Catskill NY
- 200 Amp Panel Upgrade
- EV Charger Installation Hudson Valley
- Emergency Electrical Services

---

## What Was Completed (Phase 1)

### 1. SEO Metadata Overhaul
**Scope:** 30+ static pages rewritten, 100+ CMS items verified

Every page had its SEO title, meta description, and Open Graph data rewritten from scratch.

**Pages updated:**
- **Service Pages (4):** Electrical, HVAC, Mini Split, Generator — balanced keywords with Diamond Elite and Generac branding
- **Location Pages (9):** Greene, Dutchess, Ulster, Columbia counties + Catskill, Hudson, Woodstock, Rhinebeck, Hunter — localized for each market
- **Career Pages (5):** Fixed critical issue where all 5 had generic "generator" descriptions. Now job-specific with HVAC & electrical mentions
- **Conversion Pages (6):** Contact, Reviews, Financing, Promotions, Gallery, Incentives & Rebates — CTA-focused
- **Utility Pages (7):** About, Blog, Careers, Sitemap, Privacy, Terms, Accessibility — consistent branding
- **CMS Items (100+):** Electricals (98 pages), Mini Splits (58), Generators (38), Hot Water Heaters (6), HVACs (3), Locations (9)

**Example — Home Page Title:**
- Before: `Reliable Electricians in Hudson Valley - TZ Electric Inc.`
- After: `Hudson Valley HVAC & Electrical Services | Mitsubishi Diamond Elite | TZ Electric`

**CMS fixes during audit:**
- 3 Mini Split pages had missing/inadequate meta titles and descriptions (Replacement of Ducted Systems, Central Air Heating & Cooling, Hot Water Heater Installation)
- 6 Hot Water Heater pages had weak generic metadata — all rewritten with location keywords and conversion language
- 5 Career pages had copied generator descriptions — all made unique

### 2. Schema Markup (Structured Data)
**Scope:** 7 JSON-LD scripts deployed to site header

The site previously had **zero structured data**. Seven comprehensive schema scripts were created and registered via Webflow's Custom Code system (site-level header scripts).

| # | Schema Type | Key Data |
|---|---|---|
| 1 | **LocalBusiness** | Name, address, phone, hours, geo coords, social profiles, service catalog |
| 2 | **HVACBusiness** | Mitsubishi Diamond Elite credential, mini split expertise, 4-county area |
| 3 | **Electrician** | Master Electrician license, 7-city targeting, full service list |
| 4 | **Generator Service** | Generac authorized dealer, standby installation, emergency power |
| 5 | **AggregateRating** | 5.0 stars, 200+ reviews — enables star ratings in search results |
| 6 | **FAQ** | 4 Q&As: service area, Diamond Elite, Generac partnership, financing |
| 7 | **WebSite** | Site search action, official name/URL — enables sitelinks search box |

**Technical notes:**
- All scripts are inline JSON-LD in the site header
- Webflow inline scripts have a 2000-character limit — schemas were optimized to fit
- Scripts were registered using Webflow's `data_scripts_tool` via the `add_inline_site_script` action
- All schemas pass Google's Rich Results Test

### 3. Image Alt Text Optimization
**Scope:** 95 images updated

Most images had null or generic alt text (e.g., `alt=""`, `alt="plug icon"`, `alt="Team member"`). Every image now has a descriptive, keyword-rich alt tag.

| Category | Count | Example Alt Text |
|---|---|---|
| Team Headshots | 17 | "Tyler Zitz — Owner and Master Electrician at TZ Electric Inc Hudson Valley" |
| Project Gallery | 15 | "Generac Standby Generator Installation in Ulster County by TZ Electric" |
| Products/Equipment | 20+ | "Mitsubishi Mini Split Wall-Mounted Unit — Ductless Heat Pump System" |
| Certification Badges | 10 | "Mitsubishi Diamond Elite Certified Contractor Badge — TZ Electric Inc" |
| Service/Hero Images | 15+ | "TZ Electric HVAC and Electrical Team — Serving Catskill NY and Hudson Valley" |
| Icons/UI Elements | 18 | Descriptive function labels replacing empty attributes |

**Technical method:** Updated via Webflow `asset_tool` using `update_asset` action with asset_id and alt_text parameters, processing 15–17 images per batch.

### 4. Internal Linking Architecture
**Scope:** 200+ pages connected, 3 scripts deployed, 9 location pages enhanced

Previously, the site's pages were largely isolated. A comprehensive linking architecture was built across every level.

**What was built:**

1. **Location Page Cross-Links (9 CMS pages):**
   Each location page went from 2 basic links to 15+ strategic cross-links connecting to all service pages, conversion pages (/reviews, /financing, /incentives-rebates, /promos), and other location pages with area-specific context (e.g., Hunter mentions ski lodges, Rhinebeck mentions historic homes).

2. **CMS Service Cross-Links (10 items in Services collection):**
   Complementary services connected: mini splits ↔ HVAC, generators ↔ electrical, EV chargers ↔ service upgrades, hot water heaters ↔ HVAC. Added via `service-details` rich text field.

3. **Dynamic CMS Cross-Linking Script ("Internal Cross Links"):**
   JavaScript deployed to footer. Automatically adds "Explore More Services" section on every CMS service page based on which collection the visitor is viewing. Detects URL patterns (`/electrical/`, `/generator/`, `/mini-split/`, etc.) and shows relevant complementary links.

4. **Static Page Cross-Linking Script ("Static Page Cross Links"):**
   Handles the 5 main static service pages (`/electrical`, `/hvac`, `/mini-split`, `/generator`, `/hot-water-heater`) with contextual links to related services.

5. **Breadcrumb Navigation Script:**
   Visual breadcrumbs + BreadcrumbList schema markup on all service and location pages. Improves crawlability and user orientation.

**Coverage:**
- 98 Electrical pages, 58 Mini Split pages, 38 Generator pages, 6 Hot Water Heater pages, 3 HVAC pages, 9 Location pages, 5 Static Service pages

### 5. Front-End Content & CMS Fixes
**Scope:** Home page edits, bug fixes, CMS publishing issues, UX improvements

**Home Page Subheader Update:**
- Before: "Providing Eco-Conscious Electrical Services to Homes and Businesses in Greater Catskill, NY"
- After: "Providing HVAC & Electrical Services to Homes and Businesses in Greater Catskill, NY"
- Rationale: "Eco-Conscious" doesn't target high-value keywords. "HVAC & Electrical" reinforces the 50/50 rebalance on the most visible home page element.

**Hot Water Heaters Card Description:**
- Before: "Our team provides dependable plumbing services designed to give you peace of mind."
- After: "Expert installation, repair, and maintenance for electric, hybrid, and on-demand hot water heaters in Catskill & the Hudson Valley. Enjoy reliable hot water, energy savings, and professional service you can trust."

**Bugs Resolved:**

| Bug | Root Cause | Fix |
|---|---|---|
| Raw HTML anchor tags on home page cards | 9 CMS service items had `<a href>` tags in `service-short-details` (plain text field). Tags rendered as visible text instead of links. | Cleaned all 9 items removing HTML markup, preserved descriptive content. Republished. |
| "Ductless Heat Pumps" content not publishing | CMS item had `isDraft: true` since May 2025, blocking publication. Last published 2025-05-19 but updated 2026-02-13. | Published directly via CMS API using `publish_collection_items`. |
| Hot Water Heater card not publishing from Designer | CMS-bound text edits in Webflow Designer are visual previews only — on publish, Webflow pulls data from CMS item, which had old content. | Updated content at CMS level, not Designer level. |
| Pixelated team hero image | TZ-Team-2025.avif rendering at low resolution on home page. | Fixed image settings in Webflow Designer. |

**Report UX Improvements:**
- **Accordion Default State:** Modified `TZ_Electric_SEO_Report_FINAL.html` to have all 12 toggle sections start **collapsed** on page load instead of 4 sections open by default. Improves user experience by allowing visitors to open sections one-by-one as needed. Removed `open` class from section-card divs at lines 743, 994, 1112, and 1235. (Feb 13, 2026)

---

## Webflow Technical Reference

### Site Structure

```
Platform: Webflow (hosted)
Site ID: 67ac70b9e25b6a62ed436918
Locale ID: 67ac70b9e25b6a62ed43691a
Designer URL: https://tzelectricinc.design.webflow.com
Published URL: https://tzelectricinc.com
```

### CMS Collections

| Collection | ID | Item Count | Content |
|---|---|---|---|
| **Services** | `67ac70b9e25b6a62ed436940` | 10 | Service Upgrades, Electrification, EV Chargers, Residential Wiring, Commercial Wiring, Indoor Electrical, Outdoor Electrical, Generators, Mini Splits, Ductless Heat Pumps |
| **Electricals** | `67ac70b9e25b6a62ed436940` | 98 | Individual electrical service pages |
| **Mini Splits** | `67d7cdd3a3eb4f831dc74e84` | 58 | Individual mini split/HVAC pages |
| **Generators** | (see Electricals collection) | 38 | Generator service pages |
| **Hot Water Heaters** | (in Services collection) | 6 | Hot water heater service pages |
| **HVACs** | `67d8f069eac97f65a3807680` | 3 | General HVAC pages |
| **Locations** | `67d7ccc2b1eecae2153bb8b7` | 9 | Greene, Dutchess, Ulster, Columbia counties + Catskill, Hudson, Woodstock, Rhinebeck, Hunter |

### Services Collection Fields
- `name` — Service name
- `slug` — URL slug
- `service-caption` — Short tagline
- `service-short-details` — **Plain text** field (renders on home page cards — do NOT put HTML here)
- `service-details` — **Rich text** field (supports HTML, used for full service page content and cross-links)
- `service-image` — Main service image
- `service-icon-01` — Icon for cards
- `meta-title` — SEO title
- `meta-description` — SEO description
- `Q&A 1–5` — FAQ pairs
- `elec` — Boolean flag

### Scripts Deployed (10 total)

**Header Scripts (Schema Markup — 7):**
1. LocalBusiness Schema — v1.0.0
2. Service Schema HVAC — v1.0.0
3. Electrician Schema — v1.0.0
4. Generator Schema — v1.0.0
5. AggregateRating Schema — v1.0.0
6. FAQ Schema — v1.0.0
7. Website Schema — v1.0.0

**Footer Scripts (Functionality — 3):**
8. Internal Cross Links — v1.0.0 (dynamic CMS cross-linking)
9. Static Page Cross Links — v1.0.0 (static service page cross-linking)
10. Breadcrumb Navigation — v1.0.0 (visual breadcrumbs + BreadcrumbList schema)

### Active Navigation Pages (from Navbar component)

**Services Dropdown:**
- /electrical
- /hvac (labeled "HVAC & Mini Splits")
- /generator (labeled "Generators")
- /hot-water-heater

**About Dropdown:**
- /about
- /blog
- /incentives-rebates
- /financing (page ID: `67ac70b9e25b6a62ed436915`)
- /reviews (page ID: `680a9968a7cf0fa9e554336f`)
- /careers
- /policies
- /promos

**Other:**
- /contact (in bottom toolbar)

> **Important:** Only create internal links to pages that are in the active navigation. Some pages exist in Webflow but aren't in the nav and shouldn't be linked to.

---

## Known Issues & Action Items

### Critical (Requires Tyler / Manual Action)

| # | Issue | Details | Status |
|---|---|---|---|
| 1 | **HomeAdvisor wrong address** | Shows "3423 Route 23A, Newburgh, NY" instead of "5079 Route 32, Catskill, NY 12414". NAP inconsistency hurts local pack rankings. | ⏳ Pending |
| 2 | **Yellow Pages phone mismatch** | Palenville listing shows (845) 549-9560 vs. main (518) 678-1230. Should be merged. | ⏳ Pending |
| 3 | **Missing directory profiles** | No presence on Yelp, Nextdoor, Bark, Porch, Expertise.com. Free citation opportunities. | ⏳ Pending |

**Standard NAP for all directories:**
```
TZ Electric Inc.
5079 Route 32, Catskill, NY 12414
(518) 678-1230
```

---

## Competitor Landscape

| Competitor | Threat | Key Intel | Counter-Strategy |
|---|---|---|---|
| **DS Home Services / Holdridge Electric** | 🔴 HIGH | Also Mitsubishi Diamond Elite AND Generac PowerPro Elite+. Same counties. Prominently displays both certs. | Match cert positioning in title tags. Out-content with deeper service pages and better UX. |
| **Precision HVAC** | 🟡 MEDIUM | Hyper-local city pages with census data and housing stats. Strong Catskill presence with Fujitsu mini splits. | Create landmark-context location pages. Leverage Diamond Elite over Fujitsu. |
| **Kool Temp Heating & Cooling** | 🟢 LOW | Broad regional terms. Kingston, Catskill, Coxsackie. Less nimble. | Win on specific mini split long-tail keywords and localized content. |

---

## Phase 2 Roadmap (Not Yet Started)

### High Priority
1. **AI & LLM Optimization (AGO)** — Optimize for AI Overview snippets, ChatGPT/Gemini/Perplexity discovery, conversational FAQ content, speakable schema, clean semantic HTML for AI crawlers.
2. **Competitor Keyword Gap Strategy** — Out-content DS Home Services. Replicate Precision HVAC's hyper-local city pages with community details and housing stats.
3. **NAP & Citation Cleanup** — Fix the 3 critical action items above.

### Medium Priority
4. **Blog Content Strategy** — HVAC-focused blog targeting long-tail keywords: heat pump vs. furnace, mini split sizing, NY rebate explainers, seasonal tips. 2–4 posts/month.
5. **Page Speed Optimization** — Core Web Vitals audit, defer non-critical scripts, optimize LCP, reduce CLS.

### Future Phase
6. **Google Business Profile Enhancement** — Regular posts, service photos, Q&A management, review responses, seasonal promotions.

---

## Working with This Project — Technical Notes

### Webflow MCP Integration
- **Data API tools** (CMS, pages, scripts, sites) work independently — no Designer needed
- **Designer tools** (elements, styles, components, snapshots) require the Webflow Designer to be open in a connected browser tab
- Designer MCP launch URL: `https://tzelectricinc.design.webflow.com?app=dc8209c65e3ec02254d15275ca056539c89f6d15741893a0adf29ad6f381eb99`
- Designer tab must remain in the foreground — switching away causes timeouts

### Common Gotchas Discovered During This Project

1. **CMS-bound content overrides Designer edits on publish.** If text in the Designer is bound to a CMS field, visual edits are just previews. The actual content comes from the CMS item. Always edit CMS-bound content at the CMS level.

2. **`service-short-details` is a plain text field.** Do NOT put HTML in it. It renders on home page cards and will show raw `<a href>` tags as visible text.

3. **`service-details` is a rich text field.** This is where HTML cross-links and formatted content go.

4. **CMS items in draft mode block publishing.** Even if you update content, if `isDraft: true`, publishing the site won't push changes. Check draft status via API: `list_collection_items` and look for `isDraft` flag.

5. **Webflow inline scripts are limited to 2000 characters.** Complex schemas must be minified or split across multiple scripts.

6. **Full element tree pulls cause context window exhaustion.** When working in the Webflow Designer via AI tools, avoid `get_all_elements` on large pages. Use targeted searches (grep on JSON results) or go the CMS API route instead.

7. **Publishing requires two steps:** (a) Publish CMS items via `publish_collection_items`, then (b) publish the site itself from the Webflow interface (or via `publish_site` API).

8. **Only link to pages in the active navigation.** Some pages exist in Webflow but aren't accessible to visitors. Check the Navbar component structure before creating cross-links.

### Efficient Workflow for Future SEO Updates
```
1. Use CMS API (data_cms_tool) for content changes → fastest, no Designer needed
2. Use Scripts API (data_scripts_tool) for schema/script updates → no Designer needed
3. Use Asset API (asset_tool) for image alt text → no Designer needed
4. Use Pages API (data_pages_tool) for page-level SEO metadata → no Designer needed
5. Only use Designer tools for visual/structural changes that can't be done via API
6. When using Designer: keep queries targeted, avoid full page element dumps
```

---

## Expected Results Timeline

| Timeframe | Expected Impact |
|---|---|
| **Week 1–2** (Feb 13–27) | Google recrawls site. Schema appears in Search Console. Rich results (stars, FAQ) may begin showing. |
| **Week 2–4** (Feb 27–Mar 13) | New titles/descriptions appear in SERPs. 15–30% CTR increase expected. |
| **Month 1–3** (Mar–May) | HVAC/mini split keywords see biggest ranking jumps. Location terms climb. Image search traffic increases. |
| **Month 3–6** (May–Aug) | 20–40% organic traffic increase. Better "near me" visibility. More calls and form submissions. |
| **Month 6–12** (Aug 2026–Feb 2027) | Full compound impact. Domain authority improves. Long-tail keywords across 200+ pages drive steady traffic. |

### Google Search Console Metrics to Track
- Total impressions (increase within 2–4 weeks)
- Average CTR (improvement from rewritten titles/descriptions)
- Rich results in Enhancements tab (FAQ, Review snippets)
- "Mitsubishi" and "Diamond Elite" appearing as new ranking queries
- Coverage report confirming all CMS pages indexed with no errors

---

## File Manifest

| File | Purpose |
|---|---|
| `TZ_ELECTRIC_SEO_PROJECT_README.md` | This file — universal context document for any AI/developer |
| `TZ_Electric_SEO_Report_FINAL.html` | Interactive HTML report for client (Tyler) — includes sidebar nav, collapsible sections, interactive checklists, visual timeline |
| `index.html` | GitHub Pages entry point — mirrors the main report file for web access |
| `README.md` | GitHub repository landing page with project overview and quick links |

---

---

## Recent Updates

### February 13, 2026 (Evening) — Report UX Enhancement
- Fixed accordion default state in HTML report — all sections now start closed
- Created GitHub repository README for better documentation
- Synced `index.html` with updated report file
- Repository: [github.com/cqdesignsny/TZ-SEO-Overhaul](https://github.com/cqdesignsny/TZ-SEO-Overhaul)
- Live Report: [cqdesignsny.github.io/TZ-SEO-Overhaul](https://cqdesignsny.github.io/TZ-SEO-Overhaul)

---

*Last updated: February 13, 2026 by CQ Marketing (Cesar) via Claude*
*Total sessions: 13+ across Feb 12–13, 2026*
