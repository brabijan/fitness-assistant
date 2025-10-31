# Training Plans

Zde najdeš své týdenní a mesocyklus plány.

## Struktura

```
training-plans/
├── current-week.md          ← Aktuální týdenní plán
├── mesocycle-plan.md        ← 4-6týdenní blok (optional)
└── archive/                 ← Staré plány
    ├── week-01.md
    ├── week-02.md
    └── ...
```

## Jak To Funguje

1. **Claude vytvoří `current-week.md`** každý týden
2. Obsahuje detailní plán pro každý den
3. Na konci týdne Claude archivuje do `archive/week-XX.md`
4. Vytvoří nový `current-week.md` pro příští týden

## Příklad Workflow

**Neděle večer:**
```
Ty: "Claude, udělej plán na příští týden"
Claude: *vytvoří current-week.md*
```

**Během týdne:**
```
Ty: "Jaký mám dnes trénink?"
Claude: *podívá se do current-week.md, řekne ti plán*
```

**Před tréninkem:**
```bash
cat training-plans/current-week.md
```

**Real-time adjustace:**
```
Ty: "Dnes jsem unavený, můžeme upravit?"
Claude: *upraví current-week.md podle potřeby*
```

## Mesocyklus

**Mesocyklus = 4-6týdenní blok s progresivním plánem**

Claude může vytvořit `mesocycle-plan.md` s:
- Celkovou strategií na 4-6 týdnů
- Jak bude intenzita/objem progredovat
- Cíle na konci bloku

Pak každý týden detailní plány v `current-week.md` podle mesocyklu.

---

**Tip:** Vždycky checkni `current-week.md` v neděli večer, abys věděl co tě čeká!
