# Task: Add neofetch-style stats card to GitHub profile README

Repo: `Sridattasai18/Sridattasai18` (this cloned repo)

## Step 1 — Create `neofetch.json` at the repo root

Create a new file named `neofetch.json` in the root of this repo with exactly this content:

```json
{
  "sections": [
    {
      "title": "{{username}}@github",
      "fields": [
        { "key": "Name", "value": "{{name}}" },
        { "key": "Role", "value": "B.Tech CSE (AI & Data Science), Final Year" },
        { "key": "College", "value": "Vishnu Institute of Technology" },
        { "key": "Location", "value": "{{location}}" },
        { "key": "Uptime", "value": "{{uptime}}" }
      ]
    },
    {
      "fields": [
        { "key": "Languages", "value": "{{languages}}" },
        { "key": "Currently Learning", "value": "Salesforce Dev (Apex, LWC, SOQL)" },
        { "key": "IDE", "value": "VSCode, Cursor" }
      ]
    },
    {
      "fields": [
        { "key": "Interests.AI", "value": "GenAI, Agentic AI Systems" },
        { "key": "Interests.Dev", "value": "Full-Stack Web Apps, UI/UX" }
      ]
    },
    {
      "title": "- Contact",
      "fields": [
        { "key": "Email", "value": "kaligotlasridattasai18@gmail.com" },
        { "key": "Portfolio", "value": "https://proto-folio-three.vercel.app/" },
        { "key": "LinkedIn", "value": "https://www.linkedin.com/in/kaligotla-sri-datta-sai-vithal-01bb2a321/" },
        { "key": "X", "value": "https://x.com/Sridattasai18" }
      ]
    }
  ],
  "stats": {
    "title": "- GitHub Stats",
    "rows": [
      { "left": { "key": "Repos", "value": "{{repos}}" }, "right": { "key": "Stars", "value": "{{stars}}" } },
      { "left": { "key": "Commits", "value": "{{commits}}" }, "right": { "key": "Followers", "value": "{{followers}}" } },
      { "left": { "key": "Forks", "value": "{{forks}}" }, "right": { "key": "Following", "value": "{{following}}" } },
      "loc"
    ]
  }
}
```

## Step 2 — Insert the card into `README.md`

Open `README.md`. Right after the `💫 About Me` intro paragraph block and its bullet list (i.e., right before the `## 🌐 Socials:` heading), insert this block on its own lines:

```md
<p align="center">
  <a href="https://github.com/jeantimex/neofetch-profile">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://neofetch-profile.vercel.app/api?username=Sridattasai18&theme=github-dark&config=https%3A%2F%2Fraw.githubusercontent.com%2FSridattasai18%2FSridattasai18%2Fmain%2Fneofetch.json">
      <img alt="Neofetch Profile" src="https://neofetch-profile.vercel.app/api?username=Sridattasai18&theme=github-light&config=https%3A%2F%2Fraw.githubusercontent.com%2FSridattasai18%2FSridattasai18%2Fmain%2Fneofetch.json">
    </picture>
  </a>
</p>
```

Do not modify or remove any other existing content in `README.md` (Tech Stack badges, GitHub Stats images, Socials badges, footer comment) — only add the block above in the specified location.

## Step 3 — Verify

- Confirm `neofetch.json` is valid JSON (no trailing commas, proper brackets).
- Confirm the inserted `<picture>` block appears exactly once, in the location specified.
- Do not commit/push automatically — leave changes staged for manual review.
