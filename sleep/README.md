# Sleep Screenshots

Sem ukládej své denní screenshoty spánku ve formátu `YYYY-MM-DD.png` (nebo `.jpg`).

## Jak Začít

1. Každý večer/ráno udělej screenshot své sleep tracker app
2. Ulož sem jako `YYYY-MM-DD.png`
3. Claude analyzuje kvalitu a délku spánku
4. Podle toho adjustuje intenzitu tréninku

## Formát

```
2025-11-01.png  ← Screenshot spánku z noci 31.10 → 1.11
2025-11-02.png
2025-11-03.png
...
```

## Proč Je To Důležité?

**Spánek = recovery!**

- Špatný spánek → Claude sníží intenzitu
- Dobrý spánek → můžeš push hard
- Konzistentně špatný spánek → adjustace celkového objemu

## Příklad

```bash
# Zkopíruj screenshot ze telefonu
cp ~/Downloads/sleep_screenshot.png sleep/2025-11-01.png
```

Claude pak vidí screenshot a může říct:
"Vidím že jsi spal jen 5.5h, dnes zkusme light session místo heavy tréninku."
