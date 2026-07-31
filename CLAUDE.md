# Tiff Top Community Solutions — Website

Read this before making changes. It carries context from the planning sessions.

## About the project

A 9-page informational website for **Tiff Top Community Solutions**, a 501(c)(3)
nonprofit in Columbus, Ohio serving people in reentry and recovery.

- Legal name: **Tiff Top Community Solutions** (two F's, then "Top"). Never "Tif Top" or "Tiff Top Solutions."
- Domain: TTC-solutions.org
- Address: 1511 S. High St, Columbus, OH 43207
- Phone: 614-502-0396 · Email: tiffany@ttc-solutions.org
- Hours: Monday–Friday, 10am–6pm
- Tagline: "Renew. Restore. Rebuild." / "Uniting for our future, together."

Ryan Masterson (Masterson Marketing and AI Solutions) is building this. **He is not a
developer.** Explain changes in plain English. Don't ask him to run commands, edit code
by hand, or make technical decisions without laying out the tradeoff in normal language.

## Who the site is for

Primarily **other organizations**, in this order:

1. Referral partners — case managers, probation officers, discharge planners
2. Employers — for the Second Chance Staffing program
3. Funders and grantmakers

Individuals seeking services are a secondary audience served by one page
(`looking-for-services.html`).

**There is no online intake or enrollment.** Services start with a conversation in person.

`contact.html` and `looking-for-services.html` each carry a *contact* form — added at Ryan's
request in July 2026 because the team cannot answer every phone call, and a routed message
beats a missed call. Those forms ask only: name, how to reach you, who you are / who it's
for, what you need, and an optional short message. **They must never ask about health,
treatment, recovery history, criminal record, immigration status or finances**, and the
hint text tells people not to type those details in. Do not turn either one into an
application, intake, or enrollment form. `privacy.html` describes both forms — if the
fields change, that page changes with them.

## Tech decisions

- Plain HTML, CSS, and vanilla JS. **No frameworks, no build step, no npm.**
- One file per page. Header and footer are duplicated in each file so the site works by
  opening a file directly. When the nav changes, update all pages.
- All styling lives in `css/style.css`, organized into numbered CAPS sections.
- Fonts: Big Shoulders Display (headings) + Public Sans (body), loaded from Google Fonts.
- Hosting will be Cloudflare Pages or Netlify. Donations via Givebutter or Zeffy (both free to nonprofits).

## Brand colors

| Name | Hex | Used for |
|---|---|---|
| Navy | `#0E2A56` | Headings, hero bands, footer |
| Red | `#C8102E` | Buttons, accents, CTA bands |
| Cream | `#F7F4EC` | Page background |

Defined as CSS variables at the top of `style.css`. Change them there, not inline.

## Page structure — a deliberate story arc

Nav order is the narrative and should not be rearranged without discussion:

1. `index.html` — Home *(built)*
2. `about.html` — About Us *(shell)*
3. `programs.html` — Our Programs *(built)*
4. `why-choose-us.html` — Why Choose Us *(shell)*
5. `impact.html` — Our Impact *(shell)*
6. `get-involved.html` — Get Involved *(shell)*
7. `contact.html` — Contact Us *(shell)*

Plus: `donate.html`, `employers.html` (sits under Get Involved),
`looking-for-services.html`. Still to write: `privacy.html`, `terms.html`.

Phase 2: eight program detail pages, and a filterable community resource directory
built from an existing housing-resources PDF.

## Rules that matter

**Never invent impact numbers.** The stats on the homepage are em dashes on purpose.
A funder who spots a placeholder statistic stops trusting the organization. Leave them
blank or delete the section until Ryan supplies verified counts.

**All eight programs are live** as of 31 July 2026: Transition & Reentry, Workforce
Development, Second Chance Staffing, Housing Assistance, Life Skills Training, Peer-Led
Support Groups, Peer Support Services, Case Management. Ryan confirmed that day that the
credentialed staff for the last two are in place, and the "Launching 2026" badges came off.

**Still do not print the word "certified" without checking.** Ohio's Certified Peer Recovery
Supporter credential is regulated by OhioMHAS — training, background checks, a state exam.
Removing the badges was Ryan's call about staffing; it is not the same as clearance to write
"certified peer specialists" on a funder-facing page. If a page needs that claim, confirm who
holds the credential first. A funder can check.

**No stock photography.** Photo placeholders are navy boxes that name the shot needed.
Real phone photos will replace them. Keep the design working on typography and color alone
until then.

## Writing style

- Partner-facing pages: precise and credentialed. "Trauma-informed," "person-centered,"
  and "evidence-based" are credentials to this audience — use them here.
- `looking-for-services.html`: plain, warm, roughly 6th-grade reading level. No jargon.
- Sentence case in body copy. Headings are uppercase via CSS, not typed in caps.
- Active voice. Buttons say what happens: "Donate today," not "Submit."

## Accessibility floor

Every change must hold this line: keyboard focus stays visible, `prefers-reduced-motion`
is respected, alt text on meaningful images, color contrast passes WCAG AA, and the site
works down to a 360px-wide phone.
