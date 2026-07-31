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
| `donate.html` | Donate — needs the donation form pasted in |
| `looking-for-services.html` | For people seeking help |
| `privacy.html` · `terms.html` | Legal pages |
| `css/style.css` | **All styling.** Colors, fonts, spacing, layout |
| `assets/` | Logo and photos |

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

Every navy box with a diagonal pattern is a placeholder naming the shot needed.
Phone photos are fine — real beats polished. Avoid stock photography entirely.

Shot list:
1. Tiffany or the team at the 1511 S. High St office, natural light
2. A group session or workshop in progress (backs of heads are fine — no releases needed)
3. A one-on-one conversation at a desk
4. The building exterior with signage
1
5. Two or three headshots for the team section

To use one: save it into `assets/`, then say
*"replace the photo placeholder on the homepage with assets/office.jpg"*.

---

## Before launch

- [ ] **Connect the two forms.** There is one on `contact.html` and one on
      `looking-for-services.html`. Both are built but go nowhere until a host is chosen.
      It is the same one-line fix for both — instructions are in a comment right above each
      form. Send a test message from **both** pages and confirm they arrive before launch.
- [ ] **Embed the Givebutter or Zeffy donation form on `donate.html`.** Right now the page
      shows a dashed box telling people to call instead. Step-by-step instructions are in a
      comment right above that box in `donate.html`. Make a $1 test donation before launch.
- [ ] Replace the `—` placeholders in the impact numbers with verified counts, or delete the
      section. `impact.html` is written so it works either way — it explains the method
      instead of showing figures we cannot source yet.
- [ ] Add the EIN to the footer and to the Donate page once the determination letter arrives.
      Corporate matching-gift portals ask for it, so a blank one costs real money.
- [ ] Add real photos
- [ ] Claim and fill in the Google Business Profile with matching address, phone, hours
- [ ] Apply for Google for Nonprofits (unlocks the $10,000/month Ad Grant)
- [ ] Point `TTC-solutions.org` at the host
- [x] Write and add `privacy.html` and `terms.html`
- [x] Build out Get Involved, Employers, Donate, Impact and Looking for Services

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

The site is a folder of files, so hosting is free and simple.
Recommended: Cloudflare Pages or Netlify. Drag the folder in, connect the domain, done.
Say **"help me publish this"** in Claude Code when you're ready.
