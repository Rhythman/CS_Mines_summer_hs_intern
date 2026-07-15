# Day 2: Vibe Code Your Personal Website

By the end of today, your personal website will be live on the internet at `https://your-username.github.io`.
You will not type most of the code yourself.
Instead, you will direct an AI pair programmer (GitHub Copilot) in plain English, review what it writes, and publish the result for the whole world to see.

> ⚠️ **Important:** there is homework *before* Day 2.
> Read [`guides/00_before_day2.md`](guides/00_before_day2.md) now.
> GitHub Education approval takes days (sometimes up to two weeks), so apply as soon as you can, not the night before.
> If your application is still pending on Day 2, that is okay. Copilot Free works too, and the guides cover it.

## The plan for today

| When        | What                                                                              | Roughly    |
|-------------|-----------------------------------------------------------------------------------|------------|
| Morning     | Lecture on Transformers and LLMs: how the AI you are about to use actually works. | ~2 hours   |
| Rest of day | Build and publish your personal website with GitHub Copilot.                      | ~4-5 hours |

The afternoon is publish-first, on purpose:

1. First ~30 minutes: put a simple hello-world page live at your `github.io` address. Real site, real internet, right away.
2. The rest of the afternoon: vibe code your actual site. Add your bio, projects, and style, and push updates as you go.
3. End of day: show and tell. Everyone shares their live site with the group.

Publishing first means every improvement you make afterward goes live within minutes.
No waiting until the end to find out if it works.

## The guides (follow them in order)

Guides 00 through 02 happen **before Day 2**, at home.
Guides 03 and 04 are what you do **on the day**.

Before Day 2:

- [`00_before_day2.md`](guides/00_before_day2.md) - the master checklist: accounts, installs, and what personal content to bring.
- [`01_apply_github_education.md`](guides/01_apply_github_education.md) - create your GitHub account and apply to GitHub Education (this is the step that takes days).
- [`02_setup_vscode_and_copilot.md`](guides/02_setup_vscode_and_copilot.md) - install VS Code and Git, then sign in to Copilot and check that it works.

On Day 2:

- [`03_publish_your_first_page.md`](guides/03_publish_your_first_page.md) - publish a hello-world page live at `your-username.github.io` with GitHub Pages.
- [`04_vibe_code_your_website.md`](guides/04_vibe_code_your_website.md) - direct Copilot to turn that page into your real personal site.

> 💡 **Tip:** an optional starter template lives in [`starter/`](starter/), so you do not have to build a page from a blank file.
> It saves Copilot requests if you are on the free plan, but using it is optional. Creativity is encouraged.

## Folder map

```text
day2/
├── README.md                        ← you are here
├── guides/
│   ├── 00_before_day2.md            ← pre-day checklist
│   ├── 01_apply_github_education.md ← GitHub account + Education signup
│   ├── 02_setup_vscode_and_copilot.md
│   ├── 03_publish_your_first_page.md
│   └── 04_vibe_code_your_website.md
└── starter/                         ← optional starter website template
    ├── index.html
    ├── style.css
    └── README.md
```

## What is "vibe coding"?

Vibe coding means you describe what you want in plain English, the AI writes the code, and you review the result and steer it with follow-up requests.
You are the director. The AI is a very fast assistant that sometimes gets things wrong.
That is why you still need to read the code it writes, look at the page it produces, and think about whether it did what you asked.
Clear thinking makes better prompts, better prompts make fewer retries, and on a limited free plan every wasted request counts.

One more thing to think about as the director: your site is on the public internet, and anyone can see it.
Guide [`04_vibe_code_your_website.md`](guides/04_vibe_code_your_website.md) includes a short privacy checklist. Please take it seriously.

Yesterday you trained a model.
Today you put one to work, and by tonight you will have a link you can send to anyone.
Have fun with it! 🚀
