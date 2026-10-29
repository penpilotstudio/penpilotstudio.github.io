# PenPilot Studio – RESUME

Next session yahin se shuru karo. Last update: **29 Oct 2026**

## Project kya hai
Students ke liye simple service website: student apne content / notes / practical ki photos **WhatsApp** par bhejta hai, hum saaf handwriting mein likh kar dete hain. Order, price (quote) aur payment sab WhatsApp par.

- **Live:** https://penpilotstudio.github.io
- **GitHub:** org `penpilotstudio` (owner account `vikranttyagii100`), repo `penpilotstudio/penpilotstudio.github.io` (public, branch `main`, Pages root)
- **Local folder:** `C:\Users\Aditya\Desktop\assignment-website\`
- **WhatsApp number:** +91 86303 51527 (`index.html` → `CONFIG.whatsapp`)

## Files
| File | Kaam |
|---|---|
| `index.html` | Poori website (single file: HTML + CSS + JS) |
| `robots.txt` | Search engines + AI bots (ChatGPT, Claude, Perplexity, Gemini, Apple, Bing) ko allow |
| `sitemap.xml` | Sitemap (Google + Bing mein submitted) |
| `llms.txt` | AI assistants ke liye site summary |
| `og-image.png` | WhatsApp/Instagram link preview (1200×630) |
| `favicon.svg`, `favicon.png` | Tab / Google result icon |
| `googleea2859f46d74617f.html` | **Google verification – delete mat karna** |
| `BingSiteAuth.xml` + `msvalidate.01` meta tag | **Bing verification – delete mat karna** |
| `8f6370b7042dfbc367cfd60f1c542107.txt` | **IndexNow key – delete mat karna** |

## Website ke features
- English / Hindi toggle (EN | हिं). Choice browser `localStorage` mein save hoti hai.
- Hindi translations `index.html` ke script mein `HI` object mein hain, **English text hi key hai**. English text badlo toh `HI` ki key bhi badalni padegi, warna Hindi mein woh line English hi rahegi.
- Saare order buttons WhatsApp kholte hain, pehle se likhe message ke saath (English / Hindi).
- FAQ smooth slide up/down (JS animation, 450ms timer fallback ke saath).
- Mobile: header mein sirf logo + language toggle, blue tap highlight band, 360px tak tested.
- Section order: Hero → Services → Deadline CTA → How it works → Why us → Order (WhatsApp) → FAQ → Footer (disclaimer).
- SEO: meta + canonical + Open Graph + JSON-LD (`ProfessionalService` + `FAQPage`).

## Decisions (inhe mat badalna jab tak user na bole)
- **Koi form nahi**, sirf WhatsApp. (Pehle Google Apps Script form tha, user ke kehne par hataya.)
- **UPI ya koi payment method ka naam nahi** – sirf "pay after quote".
- **Legal-safe wording:** service = customer ke diye content ki likhai / fair copy / formatting. "Assignment likh denge", "solve", "submit", "undetectable" jaise words nahi. FAQ + footer mein disclaimer hai (no original academic work, follow institution rules, under-18 parent consent).
- **Fake testimonials nahi** – user ne maanga tha, mana kiya. Sirf asli customer feedback daalna hai.

## Search / AI setup status
- **Google Search Console** (owner ka Google account – vikranttyagii100): verified, sitemap submitted, homepage indexing requested – 29 Oct 2026.
- **Bing Webmaster Tools** (same Google login): verified (meta tag), sitemap submitted, homepage indexing requested. Status 29 Oct: "Discovered but not crawled" (nayi site ke liye normal).
- **IndexNow:** homepage + llms.txt submit kiye (202 Accepted).
- **Check karna:** ~5–12 Nov 2026 ke beech Search Console → Pages aur Bing → URL Inspection mein dekhna ki index hua ya nahi.

## Pending / next ideas
1. Testimonials section (hidden until real reviews) + footer mein "Share your feedback" WhatsApp link – user ke "haan" ka intezaar.
2. Sample work gallery – user apni asli handwriting ki 3–4 photos dega.
3. Google Business Profile (Maps / local search).
4. Apna domain (jaise `penpilotstudio.in`) – optional, GitHub Pages par custom domain jod sakte hain.

## Update / deploy kaise karte hain
`git push` ka login is PC par set nahi hai (GitHub CLI installed hai, `gh auth login` nahi kiya). Ab tak browser se deploy kiya:
1. Local `index.html` (ya jo file badli) edit karo.
2. Test: folder se `python -m http.server 8765 --bind 127.0.0.1` chala kar Chrome (Windows browser) mein `http://127.0.0.1:8765/` – desktop + mobile (360px) + Hindi mode + console errors check.
3. Chrome mein `https://github.com/penpilotstudio/penpilotstudio.github.io/upload/main` → files upload → Commit changes.
4. 1–2 min baad live check: `curl -s https://penpilotstudio.github.io/?v=$RANDOM | grep "<naya text>"`.

## Background
Market research report (India, assignment / practical file service ka scope): `C:\Users\Aditya\reports\Student assignment writing service India.md`
