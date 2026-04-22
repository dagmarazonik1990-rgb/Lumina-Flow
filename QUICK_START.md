# ⚡ Quick Start — 5 minut do deploy

## 1. Fork / clone repo

```bash
git clone https://github.com/TWOJ_USERNAME/lumina-flow.git
cd lumina-flow
```

## 2. Graj lokalnie (zero setup)

```bash
# Otwórz w przeglądarce — koniec.
open web/index.html
```

## 3. Deploy na Vercel (1 klik)

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/TWOJ_USERNAME/lumina-flow&output-dir=web)

Lub ręcznie:
```bash
npm i -g vercel
vercel --prod
```

## 4. Aktywuj GitHub Pages

GitHub repo → Settings → Pages → Source: **Deploy from branch** → `gh-pages`

## 5. Setup secrets dla auto-deploy

Zobacz `docs/GITHUB_SECRETS.md`

---

## Struktura repo

```
web/          ← Gra PWA (index.html = gotowa do grania)
engine/       ← Silnik TypeScript (beam tracer, generator)
native/       ← React Native / Expo (iOS + Android)
docs/         ← Dokumentacja
.github/      ← CI/CD workflows
```

## Branch workflow

```bash
# Nowa feature:
git checkout -b feature/resonance
git push origin feature/resonance
# → otwórz PR → merge → auto-deploy ✅
```

---

**Pytania?** Otwórz Issue lub zajrzyj do `docs/SETUP.md`
