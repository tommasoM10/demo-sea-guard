# SeaGuard v2.1 – Prototype con DEMO integrata

**Novità**
- Selettore **Sorgente: Camera / Demo**
- **Demo**: video sintetico generato localmente (funziona anche senza mare). Simula una persona che sparisce per alcuni secondi → provoca pre-allerta / allerta.
- Resto invariato: ensemble COCO-SSD + MoveNet, ROI, macchina a stati, drift, log CSV, PWA offline.

## iPhone (solo con il telefono)
1. App Store → **a-Shell** (Nicolas Holzschuch).
2. Copia la cartella `seaguard_prototype_v2_1_demo` in a-Shell (Files → Condividi → Apri in a-Shell) oppure apri lo ZIP e sposta la cartella.
3. In a-Shell:
```
cd seaguard_prototype_v2_1_demo
python3 -m http.server 8080
```
4. Safari/Edge → `http://127.0.0.1:8080/` → consenti **Fotocamera** (se usi Camera).
5. In app: Sorgente = **Demo** per provare in casa, oppure **Camera** in spiaggia.

**Consiglio**: Aggiungi alla Home (Share → Add to Home) per modalità app. Il server di a-Shell deve restare attivo.

## Parametri esempio
- Mare calmo: pre 2.5s, allerta 6.0s, stato 2–3
- Mare mosso: pre 3.0s, allerta 7.0s, stato 5–6

**Avvertenza**: prototipo non certificato per uso salvavita.
