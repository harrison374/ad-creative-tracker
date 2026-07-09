# Ad Creative Tracker (live)

Auto-generated dashboard of Uscale's in-production ad creatives, pulled from ClickUp.

- **Live site:** https://harrison374.github.io/ad-creative-tracker/
- **How it updates:** the `Refresh tracker` GitHub Action runs hourly, executes `generate.py`
  (which reads the ClickUp API using the `CLICKUP_TOKEN` repo secret), regenerates `index.html`,
  and commits it. GitHub Pages serves the result.
- **Manual refresh:** Actions tab → *Refresh tracker* → *Run workflow*.
- **Rotate the ClickUp token:** Settings → Secrets and variables → Actions → update `CLICKUP_TOKEN`.

No secrets are stored in the code; the ClickUp token lives only as an encrypted Actions secret.
