# Mausam — Put it online in 5 minutes (GitHub Pages)

The whole app is one file: **`mausam.html`**. Hosting it gives you one permanent link that opens Mausam on any PC, phone, or the demo-day projector — no installs, no GPU, no server.

---

## What you need
- A GitHub account (free) — sign up at https://github.com if you don't have one.
- The file `mausam.html` from this workspace.

---

## Steps

### 1. Create the repository
1. Log in to GitHub → click **+** (top-right) → **New repository**.
2. Name it exactly: `mausam`
3. Visibility: **Public** (required for free GitHub Pages).
4. Click **Create repository**.

### 2. Upload the file
1. On the new repo page, click **uploading an existing file**.
2. Drag `mausam.html` in.
3. Click **Commit changes**.

### 3. Turn on GitHub Pages
1. In the repo: **Settings → Pages** (left sidebar).
2. Under **Build and deployment**: Source = **Deploy from a branch**.
3. Branch = **main**, folder = **/ (root)** → **Save**.

### 4. Open your permanent link
Wait ~1 minute, then open (replace `YOUR-USERNAME`):

```
https://YOUR-USERNAME.github.io/mausam/mausam.html
```

If it 404s at first, wait a minute and hard-refresh (Ctrl+Shift+R).

### 5. Verify before demo day
On the link, check:
- Home loads with real temp (not `--`) → live API works.
- Location modal → type `395007` → a PIN chip appears → India-Post lookup works.
- 🕘 icon opens alert history → persistence works.

---

## No-GitHub alternative (fastest of all)
**Netlify Drop** — go to https://app.netlify.com/drop, drag `mausam.html` into the page, get an instant public URL. No account needed for a temporary link (sign in free to keep it permanently).

---

## Demo-day tips

- **One-time onboarding per device:** your profile lives in the browser's localStorage, so each new device does the 30-second onboarding once (Outdoor + Bicycle → Start). Do this on the demo laptop *before* judges arrive.
- **QR code:** paste the URL into a QR generator, put the QR on your last slide — judges can open Mausam on their own phones. That's a wow moment.
- **Offline backup:** keep a copy of `mausam.html` on a pendrive. Double-clicking it opens the app even with no public link (it needs internet for live data, but the UI still works and explains itself).
- **If the venue Wi-Fi blocks APIs:** the app shows the "Couldn't reach the weather pipeline" card with a retry button — that's your cue to switch to your phone's hotspot and hit retry. It recovers in ~5 seconds.
