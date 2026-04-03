# mototracker-bugs

GitHub Issues-based bug report tracker for **2Wheel Tracker** (MotoTracker) iOS app.

## Admin dashboard

The admin dashboard is hosted on GitHub Pages:
**https://brianwhitman71-cell.github.io/mototracker-bugs/**

On first load it will prompt for a GitHub Personal Access Token (stored in sessionStorage only).

## Creating a PAT

1. GitHub.com → Settings → Developer Settings → Fine-grained tokens → New token
2. Repository access: **Only select repositories** → `mototracker-bugs`
3. Permissions: **Issues** → Read and write (also enables delete via GraphQL)
4. Copy the token and paste it into the dashboard prompt

## How it works

Bug reports are submitted by the iOS app directly to the GitHub Issues API. Each issue contains:
- Description
- Device model, iOS version, app version/build
- Timestamp
- Optional screenshot (uploaded via GitHub asset upload API)
