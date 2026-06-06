# Sardinia Welcome Site

Site simplu de prezentare pentru schimbul de experiență din Sardinia.

## Fișiere

- `index.html` – pagina publică
- `content.json` – textul editabil

## Cum se actualizează automat

Pagina citește `content.json` la încărcare și apoi verifică din nou la fiecare 30 de secunde.

Ca să modifici textul fără să schimbi codul, editezi doar `content.json`, de exemplu:

```json
{
  "headline": "Bun venit în Sardinia!",
  "subtitle": "Programul complet va fi disponibil în curând.",
  "status": "Revenim imediat cu programul complet."
}
```

După ce fișierul este actualizat pe server / GitHub / Vercel, vizitatorii văd automat noua versiune.

## Deploy rapid

### Vercel

1. Pui folderul într-un repo GitHub.
2. Conectezi repo-ul în Vercel.
3. Framework preset: Other / Static.
4. Output directory: gol sau `.`.

### GitHub Pages

1. Pui fișierele în repo.
2. Settings → Pages.
3. Deploy from branch → `main` → `/root`.

