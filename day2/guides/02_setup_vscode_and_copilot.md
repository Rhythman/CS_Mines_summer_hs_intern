# Get Your Laptop Ready: VS Code, Git, and Copilot

On Day 2 you will build and publish a real website, and this guide gets your laptop ready for that.
You will install two tools (VS Code and Git), sign in to GitHub Copilot, add the Live Preview extension, and check that everything works.
It takes about 20 to 30 minutes. Do it **before Day 2**, on the laptop you will actually bring to class.

> ⚠️ **Important:** the Copilot step needs a GitHub account.
> If you do not have one yet, or you have not applied to GitHub Education, do [01_apply_github_education.md](01_apply_github_education.md) first.
> The full list of everything to do before Day 2 is in [00_before_day2.md](00_before_day2.md).

## Install VS Code

VS Code is the free code editor we will use all day.
Every version downloads from the same page: <https://code.visualstudio.com/download>.

### Windows

1. Go to <https://code.visualstudio.com/download> and click the **Windows** download button.
   This gets the "User Setup" installer, which does not need administrator permission and installs just for your user account.
2. Run the downloaded file (it is named like `VSCodeUserSetup-<version>.exe`).
3. If Windows SmartScreen shows a warning, click **More info**, then **Run anyway**.
   Only do this for the genuine installer you just downloaded from code.visualstudio.com.
4. Click through the setup wizard and accept the defaults.
5. When the wizard finishes, launch VS Code.
   You should now see the VS Code Welcome page.

### macOS

1. Go to <https://code.visualstudio.com/download> and click the **Mac** download button.
   If it asks you to pick a build, **Universal** works on every Mac, whether Intel or Apple silicon.
2. Open the downloaded `.dmg` file.
3. Drag **Visual Studio Code.app** into the **Applications** folder.
4. Launch VS Code from Applications or from Spotlight.
   You should now see the VS Code Welcome page.
5. Optional: Control-click the VS Code icon in the Dock and choose **Options**, then **Keep in Dock**, so it is always one click away.

## Install Git

Git is the tool that saves versions of your work and pushes it to GitHub.
VS Code uses Git but does not install it for you, so this is a separate step.

### Git on Windows

1. Go to <https://git-scm.com/download/win> and download the Git for Windows installer.
2. Run the installer.
   If SmartScreen warns you, click **More info**, then **Run anyway**, just like before.
3. The installer shows a lot of option screens.
   Accept all the defaults and keep clicking **Next**, then **Install**.
4. When it finishes, close VS Code completely and reopen it.
   VS Code only notices Git after a restart.

### Git on macOS

Your Mac may already have Git, and if not, it knows how to install it.

1. Open the Terminal app (or the VS Code terminal, described below) and type `git --version`, then press Enter.
2. If a version number prints, you already have Git. Skip to the next step.
3. If instead a dialog pops up saying the git command requires the command line developer tools, click **Install** and agree to the prompts.
4. Wait for the download to finish.
   This can take several minutes on slow Wi-Fi, which is exactly why you are doing it before class.

### Check that Git works

Do this check inside VS Code, since that is where you will use Git on Day 2.

1. In VS Code, open the menu **Terminal**, then click **New Terminal**.
   A terminal panel opens along the bottom of the window.
2. Type `git --version` and press Enter.
3. You should see a line like `git version 2.x.x`.
   If you see "command not found" or "git not found" instead, jump to the Troubleshooting section below.

### Tell Git who you are

Git labels every save with a name and an email, and it refuses to commit until you set them.
This is a one-time setup.

1. In that same VS Code terminal, run this command with your real name in the quotes:

   ```bash
   git config --global user.name "Your Name"
   ```

2. Then run this command with your email in the quotes:

   ```bash
   git config --global user.email "you@example.com"
   ```

3. No output means it worked.

> ⚠️ **Important:** use the **same email** as your GitHub account.
> If the emails do not match, GitHub will not connect your commits to your profile.

## Turn on Copilot in VS Code

GitHub Copilot is the AI assistant that will do the heavy lifting on Day 2.
Copilot is **built into VS Code**, so there is no extension to install.
Older tutorials say "install the GitHub Copilot extension", but that advice is outdated.

1. Look at the Status Bar, the thin strip along the very bottom of the VS Code window, and find the **Copilot** icon.
2. Hover over the icon and select **Use AI Features** (you may instead see **Sign in to use Copilot**, which is the same thing).
   If you cannot find the icon, open the Command Palette with **Ctrl+Shift+P** (Windows) or **Cmd+Shift+P** (Mac) and run **GitHub Copilot: Sign in**.
3. Choose to sign in with GitHub.
   Your web browser opens to a GitHub page.
4. Sign in to GitHub if asked, then authorize VS Code.
   The browser sends you back to VS Code.
   You should now see VS Code signed in, with the Copilot icon active in the Status Bar.
5. That is it. No credit card is ever required.
   If a sign-up page asks you for payment info, you are in the wrong flow, so close it and start over from the Status Bar icon.

### What plan am I on?

What you get depends on your GitHub account.

|                    | Copilot Free                                    | Copilot Student                                                       |
|--------------------|-------------------------------------------------|-----------------------------------------------------------------------|
| Who gets it        | Anyone who signs in with a plain GitHub account | Students approved through GitHub Education who then claim the benefit |
| Code completions   | 2,000 per month                                 | Unlimited                                                             |
| Chat and agent use | 50 requests per month                           | 200 AI Credits per month                                              |
| Model choice       | Automatic only                                  | Automatic only                                                        |

If your account has no Copilot plan, signing in from VS Code automatically enrolls you in **Copilot Free**.
If your GitHub Education application was approved, claim Copilot Student first (see [01_apply_github_education.md](01_apply_github_education.md)), then restart VS Code and sign in again.
You can check which plan you are on at <https://github.com/settings/copilot>.

> 💡 **Tip:** on Copilot Free, every chat and agent message counts toward the 50 monthly requests, and the limit resets monthly, not daily.
> Day 2 is designed to work on the Free plan, but spend your requests on the website, not on chit-chat.
> Also, neither plan lets you hand-pick an AI model. Copilot chooses automatically, so do not worry if you see no model picker.

### Verify: have your first chat

1. Open Copilot Chat with **Ctrl+Alt+I** (Windows) or **Ctrl+Cmd+I** (Mac).
   You can also click the chat icon in the title bar at the top of the window, or run **Chat: Open Chat** from the Command Palette.
   A chat panel opens on the side.
2. Type something silly, like "Write a haiku about a robot that lost its Wi-Fi", and press Enter.
3. You should get a reply within a few seconds.
   If you do, Copilot is working and your laptop is ready. 🎉

## Meet the two chat modes

At the bottom of the chat box there is a dropdown where you pick **Ask** or **Agent**.
Here is the one-sentence version of each:

- **Ask** answers questions and explains things without touching your files.
- **Agent** plans the work, edits files for you, and can even run commands, asking for your approval before anything sensitive.

(An older **Edit** mode exists, but it is deprecated and hidden by default, so you will not see it.)

On Day 2 you will mostly use **Agent**, because that is the mode that builds your website while you describe what you want.
You will learn how to drive it in [04_vibe_code_your_website.md](04_vibe_code_your_website.md).

## Install the Live Preview extension

Live Preview shows your web page in a tab inside VS Code, and it refreshes every time you save.
On Day 2 you will use it constantly to check your site before you publish, starting in [03_publish_your_first_page.md](03_publish_your_first_page.md).

1. In VS Code, open the **Extensions** view with **Ctrl+Shift+X** (Windows) or **Cmd+Shift+X** (Mac).
2. In the search box, type **Live Preview** and find the one published by **Microsoft**.
3. Click **Install**.
   You should now see **Show Preview** in the menu when you right-click an HTML file in the file list.

> ⚠️ **Important:** watch out for a similarly named third-party extension called "Live Server".
> You want Microsoft's **Live Preview**.

## Optional but fun: the Copilot CLI

This section is optional and a bit more advanced.
If you skip it, Day 2 still fully works with Copilot inside VS Code.

The Copilot CLI is Copilot living directly in your terminal, with no editor at all.
You type plain English, and it answers questions, edits files, and runs commands, always asking your approval first.
It is included with **all** Copilot plans, including Copilot Free, but every task draws from the same monthly allowance as chat, so Free-plan students may want to save those requests for the website.

### Install it

The easiest installs do not need anything extra:

- **Windows:** in a terminal, run `winget install GitHub.Copilot`.
  Note that the CLI needs PowerShell 6 or newer (the modern "PowerShell" app, not the built-in "Windows PowerShell 5.1"), so if that sounds unfamiliar, feel free to skip this section and ask a helper on Day 2.
- **macOS:** if you have Homebrew, run `brew install --cask copilot-cli`.

There is also an npm install that works on every platform, but it requires **Node.js 22 or later**:

1. If you do not have Node.js, download the LTS installer from <https://nodejs.org> and run it.
2. Then run:

   ```bash
   npm install -g @github/copilot
   ```

### First run

1. In VS Code, open your project folder, then open the menu **Terminal** and click **New Terminal**.
   That terminal already starts inside your project folder, which matters because the CLI asks to trust whatever folder you start it in.
2. Run `copilot`.
   You should now see the Copilot CLI screen.
3. When the CLI asks whether to trust the folder, approve it.
4. If it says you are not logged in, type `/login` and follow the on-screen steps to authorize in your browser with your GitHub account.
5. Try one task by typing plain English at the prompt, for example: `Explain @index.html`.
   The `@` lets you point it at a file.
6. To quit, type `/exit`.
   Pressing Ctrl+C once only cancels the current action, so press it twice if you want to exit that way.

## Troubleshooting

**I cannot find any Copilot icon or extension.**
Copilot is built in, so there is nothing to install.
Update VS Code to the latest version, then look for the Copilot icon in the Status Bar at the bottom, or run **GitHub Copilot: Sign in** from the Command Palette.

**The browser sign-in never sends me back to VS Code.**
Some managed or school browsers block the redirect back to the editor.
Copy the code shown in the browser, click **Signing in to github.com...** in the VS Code Status Bar, paste it, and press Enter.

**Windows says "Git not found" even though I just installed Git.**
VS Code only detects Git on startup.
Close every VS Code window and reopen it, then run `git --version` again.

**My Mac is stuck installing "command line developer tools".**
That download is normal and can take several minutes on slow Wi-Fi.
Let it finish, then run `git --version` again.

**Chat opened in the middle of my code instead of in a side panel.**
You pressed **Ctrl+I** (or **Cmd+I**), which is inline chat, a different feature.
Press Escape, then use **Ctrl+Alt+I** (Windows) or **Ctrl+Cmd+I** (Mac) for the Chat panel.

**My school-managed laptop will not let me install things or sign in.**
Managed devices can block installers, browser redirects, or Copilot itself through an admin policy.
If you hit a wall like this, email the instructors before Day 2 so we can plan a workaround, or bring a personal laptop if you have one.

## Are you set up?

- [ ] VS Code opens to its Welcome page.
- [ ] `git --version` in the VS Code terminal prints a version number.
- [ ] You ran both `git config` commands with your name and your GitHub email.
- [ ] Copilot Chat answers when you ask it something.
- [ ] The Live Preview extension is installed.
- [ ] Optional: typing `copilot` in a terminal opens the Copilot CLI.

All boxes checked? You are ready. 🚀
On Day 2, right after the morning lecture, we go straight to [03_publish_your_first_page.md](03_publish_your_first_page.md) and put your first page on the live internet.
