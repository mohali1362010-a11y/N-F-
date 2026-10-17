# NutriFlex · جليس القوة
Private bilingual (AR RTL / EN LTR) fitness + nutrition PWA. No build step.

## Files
- index.html – the whole app (UI, calculator, food DB, workout tracker)
- manifest.json – PWA manifest
- sw.js – offline cache
- icons/ – app icons

## Run
Serve over HTTPS or localhost (service workers and install need it):
    python3 -m http.server 8080   # then open http://localhost:8080
Phone: open the URL, menu > Add to Home screen.

## Keep it private
Host on a private place only (e.g. local network, or Cloudflare Pages / Netlify with password or access policy, or a private GitHub repo + local serving). Data is stored in this browser (localStorage).

## Notes
- AI coach and meal-photo analysis only work when the page is opened inside claude.ai (the published version). Standalone they show "AI not available". To enable them elsewhere, add your own backend that calls a vision-capable model; never put an API key in the page.
- Health Connect / Zepp sync needs a native Android app; the web app has manual entry fields.
- Git: git init && git add . && git commit -m "NutriFlex" then push to a PRIVATE repo.
