# NPD UX Audit (public mirror)

A static, read-only mirror of an internal UX audit program for the National Provider Directory (NPD). It grades the NPD prototype against the shipped build, organized by customer journey, and links each journey to the persona who owns it.

## What this is
- `index.html` - audit overview with a Journey / Lens coverage toggle.
- `runs/j1.html` - a sample journey run (J1, verify a provider).
- `audit-data.json` - the data the overview reads.
- `assets/personas/` - illustrative, AI-generated persona avatars.

## What this is not
- Not a live system. There is no backend; it is a set of static files.
- Findings only. Design standards are referenced by link, not reproduced here.
- No internal data. Evidence illustrations are schematic re-creations drawn to show
  layout and status-indicator treatment. They are not screenshots of any live
  environment and contain no real provider records. Persona links open internal
  reference pages that require sign-in.

## Run locally
Open `index.html` through a static server (it fetches `audit-data.json`):

    python3 -m http.server 8000
    # then open http://127.0.0.1:8000/index.html

## Publishing
Intended to be served as a static site (for example GitHub Pages from the repo root).
