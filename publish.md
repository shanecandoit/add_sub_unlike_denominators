# Publishing from VS Code and hosting with GitHub Pages (for teachers)

This guide assumes you're a beginner and only have Visual Studio Code installed. It shows the simplest, button-driven way to publish your project to GitHub and host it with GitHub Pages using VS Code's built-in Git support and the GitHub integration.

Prerequisites

- A GitHub account (create one at https://github.com if needed)
- Visual Studio Code installed and opened on your project folder

1) Sign in to GitHub from VS Code

- In VS Code, click the Accounts icon (bottom-left) and choose **Sign in to GitHub**.
- Follow the browser-based sign-in flow and return to VS Code when prompted. This connects VS Code to your GitHub account so it can publish repositories for you.

2) Initialize a Git repository (one click)

- Open your project folder in VS Code (File → Open Folder).
- Open the Source Control view (left sidebar icon that looks like a branch).
- If your folder isn't yet a git repo, click **Initialize Repository**.
- Stage your files by clicking the **+** next to changed files or use **Stage All Changes**, then type a commit message in the box and click the checkmark to commit.

3) Publish your project to GitHub (one click)

- After your first commit, the Source Control view shows a **Publish to GitHub** button. Click it.
- Choose a repository name (the default is fine), pick **Public** so Pages can serve it, and confirm.
- VS Code will push the new repo to your GitHub account and add the remote automatically.

4) Enable GitHub Pages (via the GitHub website)

- Open the repository page on GitHub (there will be a link shown in VS Code after publishing, or visit `https://github.com/<your-username>/<repo-name>`).
- Go to **Settings → Pages**.
- Under **Build and deployment**, set **Branch** to `main` and **Folder** to `/ (root)` (this serves `index.html` from the repository root). Click **Save**.

5) Wait and visit your site

- It usually takes a few minutes. Your site URL will be:

  `https://<your-username>.github.io/<repository-name>/`

- VS Code may show the URL in the output or the Git panel link. Open that URL in a browser to see your live app.

6) Update your site using VS Code

- Make edits to `index.html` or other files in VS Code.
- In the Source Control view, stage changes and commit with a short message.
- Click the three-dot menu → **Sync Changes** or use the cloud/push icon to push your commit — GitHub Pages will redeploy automatically.

That's it! You've published your educational app and hosted it with GitHub Pages using just VS Code. You can share the URL with students or colleagues.
