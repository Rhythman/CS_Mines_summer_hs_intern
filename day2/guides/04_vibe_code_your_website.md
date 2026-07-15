# Vibe Code Your Website

Your site is live and Copilot is ready.
Now comes the fun part: spend the afternoon turning that hello-world page into a site that is unmistakably yours.
This guide is your playbook for the rest of the day, roughly 4-5 hours of building at your own pace.

Here is the whole idea of vibe coding in one line: you are the director, and the AI is the crew.
You describe what you want, Copilot builds it, and you review the result and steer.
The vision is yours.
The typing is (mostly) not.

## Start from the starter (recommended)

The course repo ships a tiny template: one `index.html` and one `style.css`, living in [`../starter/`](../starter/).
It is a plain, working personal page with obvious placeholders where your name and bio go.

Why start from it instead of a blank file?

- Your Copilot requests are limited (numbers below), and asking an AI to generate boilerplate HTML is the most boring possible way to spend them.
- A working page you can modify beats a blank page you have to imagine.
- Every prompt you save on scaffolding is a prompt you can spend on the fun stuff.

> 💡 **Tip:** the starter is a launchpad, not a ceiling. Nothing about it needs to survive the afternoon.

Here is how to get it into your site:

1. In your browser, go to the course repo: [https://github.com/Rhythman/CS_Mines_summer_hs_intern](https://github.com/Rhythman/CS_Mines_summer_hs_intern).
2. Navigate into the `day2` folder, then the `starter` folder.
3. Open `index.html` and click the copy icon near the top right of the code (two overlapping squares; the tooltip says **Copy raw file**).
   That one click copies the whole file, no selecting needed.
4. In VS Code, open your `username.github.io` folder (the one you cloned in [03_publish_your_first_page.md](03_publish_your_first_page.md)).
5. Open your existing `index.html`, delete the hello-world contents, and paste in the starter code.
6. Back in the browser, open `style.css` in the starter folder and copy it with the same copy icon.
7. In VS Code, create a new file named exactly `style.css` next to your `index.html` and paste it in.
   You should now see both files in your folder, and the starter page should appear when you preview `index.html`.
8. Read through the starter and fill in the obvious placeholders by hand: your name, your one-liner, your bio.
   You do not need AI to type your own name.
9. Preview it locally: right-click `index.html` and choose **Show Preview** (this uses the Live Preview extension you installed in [02_setup_vscode_and_copilot.md](02_setup_vscode_and_copilot.md)).
10. Commit and push using the Source Control buttons from [03_publish_your_first_page.md](03_publish_your_first_page.md).
    Within a few minutes, your live site should show the starter page with your name on it.

Prefer to build from scratch instead?
Totally allowed.
If you are confident with HTML or you have a vision the starter would fight against, delete everything and go your own way.
It is your site.

## What goes on a personal site anyway?

Think of this as a menu, not a mandate.
Pick what fits you and skip the rest.

- **Hero**: the big top section with your name and a one-liner about who you are.
- **About**: a short paragraph in your own voice, not a formal essay.
- **Projects / things I have made**: a few cards or a list, each with a name, a sentence, and a link if one exists.
- **Resume link**: a link to a PDF if you brought one, useful later for jobs and college apps.
- **Contact / links footer**: your GitHub, plus whatever public links you want to share.

Got the basics working?
Some stretch ideas:

- A dark mode toggle.
- A photo gallery of things you have built, drawn, or baked.
- A favorite-books (or games, or albums) shelf.
- A simple blog page with one first post.
- A fun custom "page not found" page.
- A custom favicon (the tiny icon in the browser tab).
- A silly easter egg that only appears if a visitor does something specific.
- An animated background that does not make anyone motion sick.

One request from us: make it weird and personal, not corporate and generic.
A site about your speedcubing times, your dog, or your pixel art beats a beige "professional portfolio" every time.
Nobody else can build your site.

## How to talk to Copilot

This is the core skill of the afternoon.
Good prompts get good pages.

### Open agent mode

1. Open Copilot Chat: press **Ctrl+Alt+I** on Windows or **Ctrl+Cmd+I** on macOS, or click the chat icon in the title bar at the top of the window.
2. In the dropdown at the bottom of the chat box, select **Agent** (the dropdown also offers **Ask**, which answers questions without changing files).
3. Type your request and press Enter.
   You should see Copilot work through your files and propose changes as highlighted edits.
4. If Copilot asks permission before running a terminal command, read what it wants to run, then approve it.
   Leave the permission level on the default that asks first.

### The playbook

**One change per request.**
Small asks get better results, and small results are easier to review.
"Add a projects section" is one request.
"Redesign my whole site" is a coin flip.

**Be specific.**
Bad: "make it better."
Good: "make the header background a dark blue gradient and the nav links white."
Copilot cannot read your mind, only your prompt.

**Point at what you see.**
If something is broken, paste the exact error message.
If something looks wrong, describe it: "the photo overflows off the right edge of the screen on my laptop."

**Reference your inspiration.**
Describe the picture in your head: "a hero section like a movie poster: full-screen photo, my name huge in the middle."
Comparisons like that give Copilot far more to work with than adjectives like "cool" or "modern."

**Review every change.**
Each edited file shows the changes as a diff, with **Keep** and **Undo** buttons on each edit.
Look at what changed, check the preview in your browser, then keep it or undo it.
You can also undo everything from one prompt at once, so a bad response never costs you more than the one request.
One exception: **Undo** only reverts file edits, so it cannot un-run a terminal command the agent already executed.
That is one more reason to read commands before approving them.
Do not blindly keep code you have not looked at.

**Ask Copilot to explain anything you do not understand.**
"Explain what this CSS rule does, line by line" costs one request, but you keep the knowledge forever.
That trade is almost always worth it.

### A worked example

Here is a realistic prompt sequence that takes the starter to a personalized site.
Adapt every word to your own taste.
These are examples, not an assignment.

1. `Change the color scheme to forest green and cream, and use a rounded friendly font for headings. Keep everything else the same.`
2. `Restyle the hero section like a movie poster: full-height, my name huge and centered, my one-liner below it in smaller italic text.`
3. `Add a projects section with a responsive grid of 3 cards. Each card has a title, one sentence, and a link. Use these projects: [your real projects here].`
4. `Add a dark mode toggle button in the top right corner. It should switch the whole page between light and dark colors and remember the choice.`
5. `On a narrow phone screen the nav links squish together. Make the layout stack vertically and stay readable on small screens.`
6. `Add an easter egg: if someone clicks my name 5 times, confetti falls.`

Notice the shape: each prompt is one change, names specifics (colors, counts, positions), and describes the goal, not the code.
Between prompts: review, preview, and push.

### One prompt, whole new look

Worried your site will look like everyone else's because half the room started from the same template?
One good art-direction prompt fixes that.
The starter only decides what is *on* the page, not what it looks like, and Copilot can re-imagine the entire look in a single request.
So spend one request early on a big restyle, before you polish any details.

Some art directions to show the range:

- `Restyle the whole page as a retro computer terminal: black background, green monospace text, and a blinking cursor after my name.`
- `Make my site look like a vintage newspaper front page: serif fonts, column layout, my name as the giant masthead.`
- `Give the page a neon arcade vibe: dark background, glowing pink and cyan accents, pixel-style headings.`
- `Restyle everything like a minimalist art gallery: huge whitespace, tiny captions, black and white with one red accent.`
- `Make it feel like a cozy scrapbook: paper-texture background, slightly tilted cards, a handwritten-style font for headings.`

One request, whole new personality.
Better yet, do not use any of these: describe the look that feels like *you*, and no one else in the room will have it.

## Do not waste your requests

Chat and agent prompts are a budget.
Spend them like allowance money, not like tap water.

**Know your budget.**

| Plan            | Ghost-text completions | Chat and agent prompts                    |
|-----------------|------------------------|-------------------------------------------|
| Copilot Free    | 2,000 per month        | About 50 per month                        |
| Copilot Student | Unlimited              | Limited, backed by 200 monthly AI Credits |

Limits reset monthly, not daily.
On Copilot Free, 50 prompts is plenty for a focused afternoon, and one careless hour of "hmm, try again" can burn through most of them.

The rules of frugality:

1. Typing text yourself is free.
   Your name, your bio, your project descriptions: just type them.
2. One focused request beats five vague ones.
   Every follow-up message is its own billed request, so ten one-line "no, try again" messages cost ten requests.
3. If a reply is 90% right, fix the last 10% by hand instead of re-rolling the whole thing.
4. Do not hunt for a model picker.
   On the Free and Student plans, Copilot selects the model automatically, so old tutorials that say "choose a model to save requests" no longer apply.
5. Use ghost text for small edits.
   The gray suggestions that appear as you type come from a separate, much larger pool (see the table).
   For a one-line tweak, start typing and let the suggestion finish the line instead of opening chat.
6. Start a new chat for each new task.
   Copilot re-reads the whole conversation every time, so a giant all-day thread gives worse answers and costs more.

## The rhythm of the afternoon

Vibe coding is a loop.
Run it over and over until the clock runs out:

1. Pick ONE improvement you want next.
2. Prompt the agent for it.
3. Review the diff and click **Keep** (or **Undo** and re-prompt).
4. Preview locally: right-click `index.html` and choose **Show Preview**.
5. Commit and push with the Source Control buttons from [03_publish_your_first_page.md](03_publish_your_first_page.md): type a short message, click **Commit**, then **Sync Changes**.
6. Refresh your live site.
   Updates usually appear in a minute or two, and can take up to 10 minutes.
7. Repeat.

> 💡 **Tip:** push often. Every push is a save point, so if a later experiment wrecks the page, your last good version is one click away on GitHub. Committing right before a big risky prompt is a pro move.

## Ground rules

- Never paste passwords, API keys, or private personal information into a Copilot prompt.
- Your site is public on the internet.
  Every privacy rule from [00_before_day2.md](00_before_day2.md) applies to everything you publish: no home address, no phone number, and only a parent-approved photo (or no photo at all).
- You are responsible for what you ship.
  Read what the AI wrote before you push it, because "Copilot did it" is not an excuse the internet accepts.
- If Copilot writes something that does not work, that is normal.
  Debugging is part of the craft, not a sign you failed.

> ⚠️ **Important:** when the agent asks to run a terminal command, actually read the command before approving it. Saying yes to things you have not read is how surprises happen.

## Stuck?

Work down this list:

1. Re-read the error message, last line first.
   It usually says exactly what went wrong.
2. Paste the exact error into Copilot and ask it to fix the problem.
3. **Undo** the change and retry with a more specific prompt.
4. Ask a neighbor, then an instructor.
   Explaining the problem out loud fixes it surprisingly often.
5. The classic: you committed early, right?
   Your last push is always there to roll back to.

## Ship it 🚀

By the end of the day, your site should be live, personal, and a little bit weird in the best way.
Show it off.
Trade URLs with your neighbors and steal their good ideas (with credit).

And here is the best part: this site does not expire when the program ends.
It lives in your GitHub account, on your URL, for free, for as long as you want it.
Keep pushing to it next week, next semester, next year.
You built this, and it is yours.
