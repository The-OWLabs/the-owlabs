# OWLabs site

The portfolio for [The-OWLabs](https://github.com/The-OWLabs), by [@vineetjk](https://github.com/vineetjk) and [@chiraghs](https://github.com/chiraghs).

Plain HTML, CSS and JavaScript. There's no build step and no dependencies, so there's nothing to install or update.

```
index.html    page structure and copy (hero, team, footer)
style.css     colors, type, layout (colors are variables at the top)
app.js        pixel owl, the flight between perches, interactions
projects.js   ← the work. Edit this to add a project.
favicon.svg   the owl, as the browser tab icon
```

## Add a project

Open `projects.js` and add an entry. The owl visits perches in the order they appear.

```js
{
  title: "Pass Reminder",
  problem: "Pings you before your monthly bus pass runs out.",
  tags: ["React", "Firebase"],
  link: "https://github.com/The-OWLabs/your-repo",
  icon: "rocket"   // bulb | gear | rocket
}
```

- With a `link`, the card shows **live** and a "View project →" button.
- With an empty `link` (`""`), the card shows **in the works**.
- The final "Your problem next?" perch is added automatically.

You can do this straight from GitHub's web editor. Edit `projects.js`, commit, and the site updates in about a minute.

## Preview locally

Open `index.html` in a browser. That's it.

## Publish on GitHub Pages (free)

1. In the The-OWLabs org, create a public repo named **`The-OWLabs.github.io`**.
2. Push these files to the root of its `main` branch.
3. In the repo, go to **Settings → Pages**. Under *Build and deployment*, pick **Deploy from a branch**, then `main` and `/ (root)`.
4. The site goes live at **https://the-owlabs.github.io**.

For a custom domain later (e.g. `owlabs.dev`), add it under Settings → Pages → Custom domain and point your DNS at GitHub Pages.

## Change the look

- **Accent color:** set `--accent` in `style.css`. The owl itself always keeps the logo colors.
- **Team:** the two member cards are in `index.html`, inside `#team`.
- **Hero copy:** lives in `index.html`, inside `.hero`.
