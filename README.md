# ARCHIE · Private OS — Deploy Guide

## Ce ai nevoie (5 minute total)

### 1. Anthropic API Key
- Du-te la: https://console.anthropic.com
- Settings → API Keys → Create Key
- Copiază cheia (începe cu `sk-ant-...`)

### 2. Deschide `src/App.jsx`
Găsește linia:
```
const ANTHROPIC_API_KEY = "YOUR_ANTHROPIC_API_KEY_HERE";
```
Înlocuiește cu cheia ta reală.

### 3. Deploy pe Vercel (gratuit)

**Opțiunea A — GitHub (recomandat):**
1. Creează un repo GitHub (privat!) și urcă fișierele
2. Du-te la vercel.com → Import Project → selectează repo
3. Deploy — gata în 2 minute

**Opțiunea B — Vercel CLI:**
```bash
npm i -g vercel
cd archie
npm install
vercel --prod
```

### 4. Instalare pe telefon

**iPhone:**
- Deschide URL-ul în Safari
- Apasă butonul Share (pătrat cu săgeată)
- "Add to Home Screen"
- Gata — apare ca aplicație nativă

**Android:**
- Deschide URL-ul în Chrome
- Meniu (3 puncte) → "Add to Home screen"
- Gata

### 5. Notificări
La prima deschidere, acceptă permisiunea pentru notificări.
ARCHIE îți va trimite notificări la ora fiecărui task din program.

---

## Securitate
⚠️ Repo-ul trebuie să fie PRIVAT — conține API key-ul tău.
Alternativ, poți folosi Vercel Environment Variables pentru mai multă securitate.

## Cost estimat
~$5-15/lună la utilizare normală (Anthropic API)
Vercel hosting: gratuit
