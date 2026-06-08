# Focus Contract Prototype

## What This Is

This project is a standalone interactive web prototype for a mobile app concept called **Focus Contract**.

It is intentionally built as a **high-fidelity browser prototype**, not a real iOS or Android app. The goal is to simulate the product experience:

- fake iPhone hardware frame
- polished mobile UI
- multi-screen flows
- stateful contract setup
- distraction intercept behavior
- dashboard, insights, and plan screens

The prototype is designed to run by opening `index.html` directly in a browser. There is no build step and no backend.

## How To Run Locally

1. Clone or download the project.
2. Open `index.html` in a desktop browser.
3. Click through the app screens inside the fake iPhone frame.

Because everything is self-contained in one HTML file, it also works offline.

## What Is Simulated

This prototype simulates:

- creating a focus contract
- choosing a task
- picking blocked distractions
- enforcing the free-plan limit of 3 blocked distractions per session
- selecting strict mode settings
- signing the contract
- running a fast demo countdown
- triggering distraction intercept overlays
- requiring reflection before early exit
- saving a completed session into the dashboard
- showing fake but realistic analytics and plan comparisons

It also uses `localStorage` to preserve the prototype state between refreshes when available.

## What Is Not Real

This is **not** a production blocker and does **not** integrate with native device controls.

The prototype does **not** implement:

- real app blocking
- Screen Time APIs
- Android accessibility or device-admin controls
- native notifications control
- backend authentication
- payments
- real account sync
- NFC or hardware features of any kind

## What A Real Native Implementation Would Require

To turn this into a real product, the team would need native platform work beyond a static web prototype.

Likely requirements would include:

- iOS and Android native app development
- platform-specific permission handling
- real distraction-blocking enforcement paths
- secure account/auth flows
- backend services for history, sync, and analytics
- subscription handling for Free vs Pro
- data models for contracts, sessions, review history, and insights
- testing for edge cases around interruptions, quits, and device state

The exact implementation path would differ significantly between iOS and Android because platform permissions and enforcement models are different.

## Deploying To GitHub Pages

This project is already structured for GitHub Pages because the entry point is `index.html` at the repository root.

Typical deployment flow:

```bash
git init
git add .
git commit -m "Create Focus Contract prototype"
git branch -M main
git remote add origin <repo-url>
git push -u origin main
```

Then in GitHub:

1. Open the repository.
2. Go to **Settings**.
3. Open **Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Select:
   - **Branch:** `main`
   - **Folder:** `/root`
6. Save.

After GitHub Pages finishes publishing, the site will be available at:

`https://<your-github-username>.github.io/<repository-name>/`
