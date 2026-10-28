# Personal Brand Portfolio Website

You're building a one-page portfolio site that is live on the internet, owned by you, and built from your own brand decisions.

AI can generate a website in seconds. What it can't do is decide who you are, who the site is for, and what a visitor should do next. That's your job. This project gives you a professionally designed starting point so you can focus on those decisions, then shows you how to use AI as an assistant you direct and check, not a designer you hand everything to.

---

## What you'll hand in

1. **Your live website link**, e.g. `https://yourusername.github.io`
2. **Your repository link**, e.g. `https://github.com/yourusername/yourusername.github.io`

Your repository must include:

- A completed `personal_brand.md`
- Every `EDIT` marker in `index.html` replaced with your own content
- Your colors and fonts set in `style.css`
- Your own headshot and three project images
- Working email and social links
- A site that passes the Quality Checklist at the bottom of this page

---

## The files

| File | What it controls | Do you edit it? |
|---|---|---|
| `personal_brand.md` | Your brand decisions: positioning, POV, colors, fonts, voice | Yes, first |
| `index.html` | The content: words, images, links | Yes, at every `EDIT` marker |
| `style.css` | The look: colors, fonts, corner roundness | Only the Control Panel at the top |
| `images/` | Your photos | Replace the placeholders |

**Content lives in `index.html`. The look lives in `style.css`.** Keeping them separate is how professional sites are built, and it means you can restyle the whole site without touching your words.

---

## Step 1: Write your brand guide (before touching the site)

Every choice on your site should trace back to a decision in `personal_brand.md`. If you skip this step, you'll end up choosing colors because they look nice instead of because they say something about you.

Take the output from your AI brand interview and use this prompt in Claude to organize it:

```
Below is the output of my personal brand interview, followed by a blank brand guide template.
Fill in the template using only what is in my interview. Where my interview doesn't answer
a section, write QUESTION: and ask me what you need to know. Do not invent details about me.

For colors, suggest hex codes that match my three brand words, and explain each choice in
one short sentence. For fonts, choose one pairing from this list: Classic Editorial,
Modern Bold, Friendly, Minimal Professional, Creative.

MY INTERVIEW:
[paste your interview output here]

TEMPLATE:
[paste the contents of personal_brand.md here]
```

Then read every line. Answer any QUESTION lines. Change anything that doesn't sound like you. **Rewrite your POV (section 5) in your own words.** That section is the one AI is worst at, because it doesn't know what you actually believe.

Keep your finished guide in a document for now. You'll paste it into your repository in Step 3.

---

## Step 2: Create your GitHub account and your copy of the site

GitHub stores your site's files and publishes them to the web for free.

1. Go to [github.com/signup](https://github.com/signup) and create an account.
   - **Choose your username carefully.** It becomes part of your website address. Use something professional, like `jordanlee` or `jordan-lee-creative`.
   - Verify your email before moving on.
2. Open the template link your instructor gives you and click the green **Use this template** button, then **Create a new repository**.
3. Name the repository **exactly** `yourusername.github.io`, using your real username in lowercase. Example: `jordanlee.github.io`. This gives you the cleanest web address.
4. Set it to **Public**, then click **Create repository**.
5. Turn on publishing:
   - Click **Settings** (top of your repository), then **Pages** (left menu).
   - Under **Build and deployment**, set Source to **Deploy from a branch**.
   - Set Branch to **main** and the folder to **/ (root)**. Click **Save**.
6. Wait one to two minutes, refresh the Pages screen, and click your link at the top. You should see the template site with placeholder text.

**Your site is now live.** Every change you save from here on goes live within a minute or two.

---

## Step 3: How to edit a file

1. In your repository, click the file name (for example `index.html`).
2. Click the **pencil icon** (top right of the file) to edit.
3. Make your changes.
4. Click the green **Commit changes** button. In the message box, describe what you changed, e.g. `Added my bio`. Click **Commit changes** again.

A **commit** is a saved version. GitHub keeps every one, so you can always go back.

**Start by pasting your brand guide:** open `personal_brand.md`, click the pencil, replace everything with your finished guide, and commit.

### The one rule for editing `index.html`

Change only the words **between** the tags. Leave anything inside `< >` alone.

```
<h1>Your Name</h1>        ✔ becomes   <h1>Jordan Lee</h1>
<h1>Your Name</h1>        ✘ not        <Jordan Lee>
```

Lines that start with `<!--` and end with `-->` are instructions for you. Visitors never see them. You can leave them in.

Work top to bottom through every `EDIT` marker, using your brand guide as the source.

---

## Step 4: Set your colors and fonts

### Colors

Open `style.css`. At the top is the **Control Panel**. Replace each hex code with the one from your brand guide (section 8). Commit, wait a minute, and refresh your site.

Check that your text is easy to read on your background. Paste your text and background hex codes into [webaim.org/resources/contrastchecker](https://webaim.org/resources/contrastchecker/). Aim for a **Pass** on "WCAG AA: Normal Text." Check three pairs: **text on background**, **muted text on background**, and **accent on background** (your accent colors the small section labels).

### Fonts

Changing fonts takes **two edits**: the link in `index.html` and the font names in `style.css`. Pick one pairing below and copy both lines exactly.

**Classic Editorial** (the default): elegant, thoughtful, established

- `index.html` font line:
  `<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">`
- `style.css`:
  `--font-heading: "Playfair Display", Georgia, serif;`
  `--font-body: "Inter", Arial, sans-serif;`

**Modern Bold**: confident, energetic, business-ready

- `index.html` font line:
  `<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Open+Sans:wght@400;500;600&display=swap" rel="stylesheet">`
- `style.css`:
  `--font-heading: "Montserrat", Arial, sans-serif;`
  `--font-body: "Open Sans", Arial, sans-serif;`

**Friendly**: warm, approachable, upbeat

- `index.html` font line:
  `<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600;700&family=Nunito:wght@400;500;600&display=swap" rel="stylesheet">`
- `style.css`:
  `--font-heading: "Poppins", Arial, sans-serif;`
  `--font-body: "Nunito", Arial, sans-serif;`

**Minimal Professional**: calm, credible, clean

- `index.html` font line:
  `<link href="https://fonts.googleapis.com/css2?family=Fraunces:wght@600;700&family=DM+Sans:wght@400;500;600&display=swap" rel="stylesheet">`
- `style.css`:
  `--font-heading: "Fraunces", Georgia, serif;`
  `--font-body: "DM Sans", Arial, sans-serif;`

**Creative**: inventive, modern, a bit unexpected

- `index.html` font line:
  `<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Work+Sans:wght@400;500;600&display=swap" rel="stylesheet">`
- `style.css`:
  `--font-heading: "Space Grotesk", Arial, sans-serif;`
  `--font-body: "Work Sans", Arial, sans-serif;`

### Corner roundness

`--radius` controls how rounded buttons, photos and cards are. `0px` reads sharp and formal; `24px` reads soft and friendly. Match it to your brand words.

---

## Step 5: Add your images

Your site expects four images in the `images` folder with these **exact** names, all lowercase:

| File name | What it is | Shape that works best |
|---|---|---|
| `headshot.jpg` | Your photo | Portrait (taller than wide) |
| `project1.jpg` | Image for project 1 | Landscape (wider than tall) |
| `project2.jpg` | Image for project 2 | Landscape |
| `project3.jpg` | Image for project 3 | Landscape |

To replace a placeholder:

1. Rename your photo on your computer to the exact name above.
2. In your repository, open the `images` folder.
3. Click **Add file**, then **Upload files**. Drag your photo in.
4. Click **Commit changes**. Your photo replaces the placeholder because it has the same name.

**Common problems**

- **Photo doesn't show up?** The name must match exactly. `Headshot.jpg`, `headshot.JPG` and `headshot.jpeg` will not work.
- **iPhone photo ends in `.HEIC` or `.png`?** Convert it to JPG first. [squoosh.app](https://squoosh.app) does this for free, and also shrinks large files.
- **Site loads slowly?** Keep each image under 1 MB. Squoosh can do this too.

Then update the `alt` text for each image in `index.html` so it describes the actual photo.

---

## Step 6: Use AI as your assistant, not your designer

You're allowed, and encouraged, to use AI on this project. The skill you're practising is **directing** AI and **checking** its work. Three rules:

1. **You decide, AI drafts.** Every draft gets edited until it sounds like you.
2. **One change at a time.** Ask for one specific thing, paste it, check the site, then move on.
3. **Never paste what you haven't read.** If you can't explain what it changed, don't use it.

### Drafting your content

```
I'm filling in a portfolio website template. Below is my brand guide.
Draft the text for each of these, using only what is in my brand guide,
in the voice described in section 7. Respect the length in brackets.

- Hero label [3–6 words]
- Hero tagline [1 sentence]
- About headline [under 10 words, a statement, not "About Me"]
- About paragraphs 1, 2 and 3 [2–3 sentences each]
- Project descriptions 1, 2 and 3 [1–2 sentences each: what, my role, the result]
- Contact headline [under 6 words]
- Contact sentence [1–2 sentences]

Do not invent achievements, numbers or experiences that aren't in my brand guide.

MY BRAND GUIDE:
[paste personal_brand.md]
```

### Asking for a design change

Vague requests get vague results. Be specific about **what**, **where**, and **why**.

| ✘ Vague | ✔ Specific |
|---|---|
| "Make it look better." | "In my style.css, make the skills section use my accent color for the borders instead of primary, because I want the skills to stand out more." |
| "Fix the projects." | "My project cards show three across on desktop. I want two across on desktop and one on phones. Show me only the lines in style.css I need to change." |

Always ask for **only the lines to change**, not the whole file. Then find those lines yourself and replace them. This is how you learn where things live.

### If something breaks

Every commit is saved. Click the file, then **History** (top right). Click an earlier commit, open the file, and copy the old version back in.

---

## Quality Checklist

Before you submit, check every item.

**Brand**

- [ ] Your positioning sentence is in the hero, and a stranger would understand it
- [ ] Your colors, fonts and photos match your three brand words
- [ ] The About section includes your POV, written in your own words
- [ ] The main button asks for the one action in your brand guide

**Content**

- [ ] No placeholder text remains anywhere (search the page for "Your Name" and "Skill One")
- [ ] The browser tab shows your name, not "Your Name"
- [ ] Each project says what you did, your role, and the result
- [ ] No spelling or grammar errors (read it out loud)

**Function**

- [ ] Every link and button works, including email and every social link
- [ ] All four images are yours and load properly
- [ ] Every image has alt text that describes it
- [ ] Text passes the contrast check

**Phone test**

- [ ] Open your site on your phone. Nothing is cut off, overlapping or too small to read.

---

## After this class

Your site is yours. It keeps running for free as long as your GitHub account exists. Update it whenever you finish a project, change your goals, or refine your brand. A portfolio that's six months out of date sends a message too.
