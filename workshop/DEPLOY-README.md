# Cowork Workshop page — how to publish it

The workshop is a single file: `workshop/index.html`, already placed in your website repo folder next to your main `index.html`. Because your site deploys through GitHub and Vercel, publishing it is the same push you already do for site changes.

## Set your passcode first (30 seconds)

1. Open `workshop/index.html` in any text editor.
2. Near the bottom, find this line inside the `<script>` section:

   `var PASSCODE = "stonepath";`

3. Change `stonepath` to whatever code you want to give the team. Save the file.

Note: this passcode keeps casual visitors out. It is light protection, not a lock. Anyone technical could view the page source and find it. That is fine for workshop material. If you ever need real protection, Vercel offers true password protection on a paid plan and I can set that up.

## Publish it

1. Commit and push the `workshop` folder to your GitHub repo (the same one Vercel watches for stonepathhq.com).
2. Vercel redeploys automatically in a minute or two.
3. Your page is then live at: **stonepathhq.com/workshop**

That URL is not linked from your main site, so only people you send it to will find it.

## Only the workshop is protected, not your whole site

The passcode lives entirely inside this one file (`workshop/index.html`). Nothing in it touches your homepage or any other page. As long as the file sits in a `workshop` folder, only **stonepathhq.com/workshop** asks for a passcode, and the rest of stonepathhq.com behaves exactly as before.

If you visit **stonepathhq.com** (the root) and see the passcode screen, that means this file got placed at the site root instead of in a `workshop` folder. Fix: make sure your normal homepage `index.html` is at the repo root, and this file is at `workshop/index.html`, then redeploy.

## Use it locally instead (no publishing)

You do not have to publish it at all. To run it on your laptop for the session, just double-click `index.html` and it opens in your browser, passcode and all. Same file, works offline.

## What's on the page

- **Setup:** a 3-item checklist (Claude subscription, desktop app, Chrome extension). The team checks these off, which unlocks the next two steps.
- **Learn:** a Cowork cheat sheet (what Cowork is, your STARTA framework, vague-vs-clear prompts, starter prompts) and the 3 lessons, adapted from the AI@GSB originals for a Cowork audience.
- **Try It:** the two live tasks, "Never miss a lead" and "Build a lead-capture page," each with steps and a copy-ready prompt built around MPHS.

Credit to Alfredo Mendez and the AI@GSB Claude Code Workshop appears in the footer, linked, on every view.
