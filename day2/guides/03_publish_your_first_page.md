# Publish Your First Page

In the next 30 minutes, your website goes live on the real internet at your own address.
The plan is publish plain first, make it awesome after: if publishing works now, nothing can go badly wrong at 4pm when you are polishing the final version.
By the end of this guide your hello-world page will be live at `https://your-username.github.io`, and a copy of it will be on your laptop, ready for the afternoon.

This guide assumes you finished [00_before_day2.md](00_before_day2.md) and [02_setup_vscode_and_copilot.md](02_setup_vscode_and_copilot.md): you have a GitHub account and VS Code with Git installed.

## What is GitHub Pages?

GitHub Pages is free website hosting built into GitHub.
It works for every account, so you do not need GitHub Education approval for this part.
The rule is simple: if you own a repository named exactly `your-username.github.io`, GitHub serves its files as your personal site at `https://your-username.github.io`.
Every time you push new files to that repository, your live site updates a couple of minutes later.

## Step 1: Create your special repository

1. Go to [github.com](https://github.com/) and sign in.
2. Click the **+** icon in the upper-right corner and select **New repository**.
3. If there is an **Owner** dropdown, make sure your own username is selected.
4. In the repository name field, type `your-username.github.io`, replacing `your-username` with your **actual GitHub username**.
   For example, if your username is `octocat`, the repository must be named `octocat.github.io`.
5. Select **Public**.
   On a free account, the site only publishes if the repository is public.
6. Turn the **Add README** toggle to **On**.
7. Click **Create repository**.
   You should now see your new repository's page, with a README file in it.

> ⚠️ **Important:** the repository name must be EXACTLY `your-username.github.io`, all lowercase, with your real username.
> If your username contains capital letters, write it in lowercase here.
> Any other name (a typo, `my-website`, `Octocat.github.io`) silently creates a different kind of site at a longer address instead of your main one.
> Double-check the spelling before you click create.

## Step 2: Create index.html in your browser

No editor needed yet.
You will create your homepage right in the browser.

1. On your repository's page, click the **Add file** dropdown, then click **Create new file**.
2. In the file name box, type `index.html` exactly.
   All lowercase: `Index.html` will not work, because the name is case sensitive.
3. Paste this into the file contents box, and swap in your first name:

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width, initial-scale=1">
       <title>YOUR-NAME's Website</title>
     </head>
     <body>
       <h1>Hello, world! I'm YOUR-NAME. 👋</h1>
       <p>This is my corner of the internet.</p>
       <p>Built at the CS@Mines summer program. Check back this afternoon, it's about to get way better.</p>
     </body>
   </html>
   ```

4. Click **Commit changes...** in the top right.
5. In the dialog that pops up, you can edit the **Commit message** if you like (the suggested one is fine).
6. Leave **Commit directly to the `main` branch** selected, then click **Commit changes**.
   You should now see `index.html` listed in your repository's files.

> 💡 **Tip:** this page is on the public internet, so your first name is plenty.
> No last name required, and never your address, phone number, or school schedule.
> The privacy checklist in [00_before_day2.md](00_before_day2.md) applies from this moment on.

## Step 3: Watch it go live

GitHub now builds and deploys your site automatically.
Here is how to watch it happen.

1. Click the **Actions** tab at the top of your repository.
   You should see a workflow run called **pages build and deployment**, either running or already finished with a green checkmark.
   If the list is empty, that is fine - do the next two steps first, then come back.
2. While you wait, confirm the publishing settings: click the **Settings** tab, then in the left sidebar under **Code and automation**, click **Pages**.
3. Under **Build and deployment**, the **Source** should be **Deploy from a branch**, the branch should be **main**, and the folder should be **/ (root)**.
   That is usually set automatically for this special repository, but if anything looks different, fix it and click **Save**.
4. Once the Actions run shows a green checkmark, open a new browser tab and go to `https://your-username.github.io` (your real username).

You should see your hello-world page, live on the internet. 🎉
Anyone in the world can visit that address right now.
Send it to someone.

A few timing notes:

- The first deploy usually takes 1 to 2 minutes, but it can take up to 10.
  If you see a 404, wait a bit and try again before assuming something is wrong.
- Every future update also takes a couple of minutes to appear.
- If your browser keeps showing the old version after an update, it is probably a cached copy.
  Try a private or incognito window, or clear your browser's cache.

> 💡 **Tip:** your website lives at `https://your-username.github.io`.
> The repository page at `github.com/your-username/your-username.github.io` is where the *files* live, not the site itself.
> Bookmark both, and do not mix them up.

## Step 4: Clone it to your laptop

Right now your site only exists on GitHub.
To let Copilot work on it this afternoon, you need a copy on your laptop.
That copy is called a clone, and VS Code can make it without touching a terminal.

1. Open VS Code, with no folder open.
2. Click the **Source Control** icon in the Activity Bar on the left (or press **Ctrl+Shift+G**, same keys on Windows and Mac).
3. Click the **Clone Repository** button.
   If you do not see the button, open the Command Palette and run **Git: Clone** instead.
4. Choose **Clone from GitHub**.
5. If prompted, sign in: your browser opens, you select **Sign In** and authorize, and the browser sends you back to VS Code.
6. A searchable dropdown of your repositories appears.
   Pick `your-username/your-username.github.io`.
7. Choose a folder on your laptop to store the project (something easy to find, like Documents).
8. When VS Code asks whether to open the cloned repository, click **Open**.
   You should now see `index.html` and `README.md` in the Explorer panel on the left.

> 💡 **Tip:** on some school-managed browsers, the sign-in page never bounces you back to VS Code.
> If that happens, copy the code or token the browser shows you, click **Signing in to github.com...** in VS Code's Status Bar at the bottom, paste it, and press Enter.

## The edit-publish loop you will use all day

Everything this afternoon is this one loop, repeated:

1. Edit files in VS Code (by hand, or by asking Copilot).
2. Check the result locally.
   Right-click `index.html` in the Explorer and choose **Show Preview** to see it inside VS Code (this uses the Live Preview extension from [02_setup_vscode_and_copilot.md](02_setup_vscode_and_copilot.md)).
   Or double-click the file in File Explorer or Finder to open it in your browser, and refresh after each save.
3. When it looks right, open the **Source Control** view.
   Your changed files are listed there.
4. Type a short message describing the change in the commit message box, like `Make the heading friendlier`.
5. Click **Commit**.
   If VS Code asks whether it should commit all your changes because none are staged, click **Yes**.
   That is exactly what you want.
6. Click **Sync Changes** to push your commit to GitHub.
7. Wait a couple of minutes, then refresh `https://your-username.github.io`.
   Your change is live.

Do a practice run right now so the loop is muscle memory before Copilot enters the picture:

1. In VS Code, open `index.html` and change one word.
   For example, change `Hello, world!` to `Hello, Colorado!`.
2. Save the file.
3. Preview it locally and confirm the new word shows up.
4. Commit with a message like `Practice edit`, then click **Sync Changes**.
5. Wait a couple of minutes, refresh your live site, and watch your edit appear on the internet.

> ⚠️ **Important:** if your commit fails with a message about `user.name` and `user.email`, Git does not know who you are yet on this laptop.
> Run the two one-time setup commands from [02_setup_vscode_and_copilot.md](02_setup_vscode_and_copilot.md), then commit again.

## If your site is not showing up

Getting a 404 or a blank page?
Work down this list, and one of these will be it:

1. **Repository name typo.**
   The repository must be named exactly `your-username.github.io`, all lowercase.
   Any other name puts your page at `https://your-username.github.io/repository-name` instead of the main address.
   Fix the name in the repository's **Settings** tab so it matches exactly.
2. **The repository is Private.**
   On a free account, private repositories do not publish, and there is no clear error telling you so.
   Go to **Settings** > **General**, scroll to the Danger Zone, and use **Change repository visibility** to make it **Public**.
3. **No `index.html` at the top level.**
   The file must be named `index.html` (lowercase, case sensitive) and sit at the root of the repository, not inside a folder.
   If you only have a README, you will see a plain rendered README page instead of your HTML.
4. **Wrong publishing settings.**
   In **Settings** > **Pages**, under **Build and deployment**, confirm Source is **Deploy from a branch**, the branch is **main**, and the folder is **/ (root)**.
5. **It just has not deployed yet.**
   Deploys can take up to 10 minutes.
   Check the **Actions** tab for the **pages build and deployment** run, and check [githubstatus.com](https://www.githubstatus.com/) if GitHub itself is having a bad day.
6. **Your browser cached an old version.**
   Open the address in a private or incognito window, or clear your browser's cache.

Still stuck after all six?
Wave down an instructor.
This is exactly what we are here for.

## Done. Now make it yours

You have a live website and the full edit-publish loop under your fingers.
Time for the fun part: head to [04_vibe_code_your_website.md](04_vibe_code_your_website.md) and start directing Copilot.
If you want a head start instead of a blank page, the optional template in [../starter/](../starter/) is ready to copy in. 🚀
