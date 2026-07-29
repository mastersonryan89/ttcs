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

| File / folder | What it is |
|---|---|
| `index.html` | Homepage — fully built |
| `programs.html` | Our Programs — fully built |
| `about.html` | About Us — shell, next to build |
| `why-choose-us.html` | Why Choose Us — shell |
| `impact.html` | Our Impact — shell |
| `get-involved.html` | Get Involved — shell |
| `employers.html` | Employer Partnerships — shell |
| `contact.html` | Contact Us — shell |
| `donate.html` | Donate — shell |
| `looking-for-services.html` | For people seeking help — shell |
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
5. Two or three headshots for the team section

To use one: save it into `assets/`, then say
*"replace the photo placeholder on the homepage with assets/office.jpg"*.

---

## Before launch

- [ ] Replace the `—` placeholders in the impact numbers with verified counts, or delete the section
- [ ] Add EIN and 501(c)(3) determination language to the footer and Donate page
- [ ] Embed the Givebutter or Zeffy donation form on `donate.html`
- [ ] Write and add `privacy.html` and `terms.html`
- [ ] Add real photos
- [ ] Claim and fill in the Google Business Profile with matching address, phone, hours
- [ ] Apply for Google for Nonprofits (unlocks the $10,000/month Ad Grant)
- [ ] Point `TTC-solutions.org` at the host

---

## Publishing

The site is a folder of files, so hosting is free and simple.
Recommended: Cloudflare Pages or Netlify. Drag the folder in, connect the domain, done.
Say **"help me publish this"** in Claude Code when you're ready.
