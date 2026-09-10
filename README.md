# Tiff Top Community Solutions — Website

Plain HTML and CSS. No build step, no framework, no plugins to update.
Double-click any `.html` file to open it in your browser and see the site.

---

## Working on this in Claude Code

Open Claude Code in this folder and describe what you want in normal English.
You never need to touch the code yourself.

Things you can say:

- "Make the hero on the homepage shorter"
- "Change the red to a deeper shade everywhere"
- "Add a section to the About page for our board members"
- "The programs page cards should be 4 across on desktop"
- "Replace the photo placeholder on the homepage with assets/office.jpg"
- "Build out the Contact page using the layout from the blueprint"
- "Undo that, go back to how it was before"

If something looks wrong, describe what you see: *"the menu overlaps the logo on my
phone"* is enough. You don't need to know why.

---

## Where things live

All nine pages plus the two legal pages are now written. Nothing is a placeholder shell
any more.

| File / folder | What it is |
|---|---|
| `index.html` | Homepage |
| `about.html` | About Us |
| `programs.html` | Our Programs |
| `why-choose-us.html` | Why Choose Us |
| `impact.html` | Our Impact |
| `get-involved.html` | Get Involved |
| `employers.html` | Employer Partnerships |
| `contact.html` | Contact Us |
| `donate.html` | Donate — carries the live Givebutter form |
| `looking-for-services.html` | For people seeking help |
| `privacy.html` · `terms.html` | Legal pages |
| `thank-you.html` | Where both forms land after someone hits send |
| `404.html` | Shown if someone follows a broken link |
| `css/style.css` | **All styling.** Colors, fonts, spacing, layout |
| `assets/` | Logo and photos |
| `robots.txt` · `sitemap.xml` | Tell Google what to list. Not seen by visitors |
| `netlify.toml` | Hosting settings. You should not need to touch it |

The header and footer are copied into each page. That means the site works by just
opening a file — no server needed. When the menu changes, tell Claude Code
**"update the header on every page"** and it will edit all of them at once.

---

## Brand

| | |
|---|---|
| Navy | `#0E2A56` |
| Red | `#C8102E` |
| Cream background | `#F7F4EC` |
| Headline font | Big Shoulders Display |
| Body font | Public Sans |

All defined at the top of `css/style.css` under **BRAND SETTINGS**.
Change one value there and it updates across the whole site.

---

## Photos we still need

**The placeholders are currently hidden**, so the live site shows no empty photo boxes.
They are all still in the pages — three rules at the end of the PHOTO PLACEHOLDERS
section of `css/style.css` just stop them being drawn. Say *"show the photo placeholders
again"* to see them while you are working out what to shoot.

Phone photos are fine — real beats polished. Avoid stock photography entirely.

Shot list:
1. Tiffany or the team at the 1511 S. High St office, natural light
2. A group session or workshop in progress (backs of heads are fine — no releases needed)
3. A one-on-one conversation at a desk
4. The building exterior with signage
5. Two or three headshots for the team section

To use one: save it into `assets/`, then say
*"replace the photo placeholder on the homepage with assets/office.jpg"*. A real photo
shows up straight away — the hiding rule only applies to the empty placeholders.

---

## Before launch

- [ ] **Turn on form notification emails, then test both forms.** The forms are connected to
      Netlify now, but Netlify only *collects* messages — it does not email them to anyone until
      you say so. In Netlify go to **Forms › Form notifications**, add Tiffany's address, and do
      it for both `contact` and `services`. Then send a real test message from **both** pages on
      the live site and confirm it arrives. Forms do not work when you open the file on your own
      computer — only once published.
- [x] ~~**Finish Givebutter account setup and publish the campaign.**~~ Done — the campaign
      "Support Stability for Neighbors in Need" is published and Givebutter is accepting
      transactions (card, digital wallet, PayPal, Venmo and Cash App). One-time and monthly
      giving are both switched on, with one-time as the default.
- [ ] **Make a $1 test donation and confirm the receipt email arrives.** Nobody has put a real
      card through the form yet. Give $1 to yourself on the published site, check the receipt
      lands, then refund it in Givebutter. This is the last thing standing between the Donate
      page and launch.
- [ ] **Decide on the optional tip prompt.** It is currently **on**, so after choosing an amount
      donors are asked to add a tip for Givebutter on top of their gift. Cover-the-fees is on
      too, which is normal. Leave both or switch the tip off in the campaign's payment settings
      — either is fine, but decide on purpose rather than by default.
- [ ] Replace the `—` placeholders in the impact numbers with verified counts, or delete the
      section. `impact.html` is written so it works either way — it explains the method
      instead of showing figures we cannot source yet.
- [ ] Add the EIN to the footer and to the Donate page once the determination letter arrives.
      Corporate matching-gift portals ask for it, so a blank one costs real money.
- [ ] Add real photos *(not a launch blocker — the placeholders are hidden)*
- [ ] Claim and fill in the Google Business Profile with matching address, phone, hours
- [ ] Apply for Google for Nonprofits (unlocks the $10,000/month Ad Grant)
- [ ] Point `TTC-solutions.org` at Netlify — see **Publishing** below
- [x] Write and add `privacy.html` and `terms.html`
- [x] Build out Get Involved, Employers, Donate, Impact and Looking for Services
- [x] Hide the photo placeholders so the site reads as finished without photos
- [x] Connect both forms to Netlify, with a `thank-you.html` page after sending
- [x] Add `404.html`, `robots.txt` and `sitemap.xml`

### Things to check with Tiffany

Each of these is marked with a **"NOTE FOR RYAN"** comment in the file, so you can say
*"show me the notes for me in employers.html"* and Claude Code will read them out.

| File | What to confirm |
|---|---|
| `get-involved.html` | The six volunteer roles; whether volunteers need a background check or references; what in-kind donations she has room to store |
| `employers.html` | How much of the tax-credit and bonding paperwork we actually help employers with. The page currently says we help them look into it, not that we file it |
| `looking-for-services.html` | Whether people really can walk in without an appointment during office hours; any local Franklin County crisis numbers she wants added; who gets the messages from the new form. **The page promises a reply within one business day** — someone has to actually check it every workday for that to stay true |
| `donate.html` | What things actually cost, so we can add real dollar amounts. No made-up "$25 buys…" lines are on the page |
| `impact.html` | Nothing to confirm — but do not let anyone fill the numbers in with estimates |

---

## Publishing

The site is a folder of files, so hosting is free. We are using **Netlify**, and keeping
the domain registered where it already is, at **Squarespace**.

Two different jobs, often confused:

- **Squarespace registers the domain.** It owns the name `TTC-solutions.org`. Keep it there.
- **Netlify hosts the site.** It serves the actual pages. Free, and no monthly bill.

Squarespace *also* sells website hosting, but it is a closed builder — there is no way to
give it this folder. Hosting the site there would mean rebuilding all fourteen pages by
hand inside their editor and paying roughly $16–25 a month. We are not doing that.

### Step 1 — put the site on Netlify

1. Make a free account at **netlify.com**.
2. Choose **Add new site › Deploy manually** and drag this whole folder onto the page.
3. It goes live in about thirty seconds at a temporary address like
   `random-name-12345.netlify.app`. Open it and click through every page.
4. Rename it to something sane under **Site configuration › Change site name**.

To publish a change later, drag the folder in again. It replaces what is there.

### Step 2 — point the domain at it

1. In Netlify: **Domain management › Add a domain**, and enter `ttc-solutions.org`.
2. Netlify will show you the exact DNS records to create. **Copy what it shows you** —
   do not use records written down anywhere else, including here, because they change.
3. In Squarespace, open the settings for `TTC-solutions.org` and find **DNS settings**.
   Add the records Netlify gave you.
4. Wait. It usually takes under an hour, sometimes up to a day. Netlify turns on the
   padlock (the HTTPS certificate) by itself once the domain resolves — free, nothing to buy.

### Step 3 — before you tell anyone

Work the **Before launch** checklist above. The two that genuinely block a launch are the
**form notification emails** and the **$1 test donation**. A site that quietly swallows
messages from someone in reentry is worse than no site at all, and a donation form nobody
has put a real card through is a promise you have not checked.

Say **"help me publish this"** in Claude Code if you get stuck on any step.
