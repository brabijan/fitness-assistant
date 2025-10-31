# AI Fitness Trenér 🏋️

Vítej v systému tvého osobního AI fitness trenéra! Tento systém ti pomůže dosáhnout tvých fitness cílů prostřednictvím inteligentního plánování, real-time asistence během tréninků a průběžného sledování pokroku.

## 🎯 Tvoje Cíle

- **Váhový pokles:** 103kg → 85kg (cca -18kg)
- **Kalistenické skills:** Muscle up, front lever, pistol squat, human flag, planche
- **Vytrvalost:** Běh a výstupy na Kleť
- **Ochrana svalové hmoty** během deficit fáze

## 🚀 Quick Start

### 1. První spuštění - Onboarding

Před tím, než začneš používat AI trenéra, musíš vyplnit základní informace:

```bash
# Otevři onboarding assessment
cat onboarding/initial-assessment.md
```

Vyplň všechny sekce v `onboarding/initial-assessment.md`. Claude ti pak na základě těchto dat vytvoří:
- Personalizovaný tréninkový plán
- Baseline metrics pro tracking pokroku
- Progresivní systém směřující k tvým cílům

### 2. Denní použití

#### Ráno - Přidání spánku
```bash
# Přidej screenshot spánku do složky sleep/
cp /cesta/k/screenshotu.png sleep/$(date +%Y-%m-%d).png
```

#### Před tréninkem - Zkontroluj plán
```bash
cat training-plans/current-week.md
```

#### Během tréninku - Real-time asistence

Otevři Claude a začni komunikovat průběžně:

**Příklad konverzace:**
```
Ty: "Dnes začínám tréninkem horní části těla podle plánu"

Claude: "Výborně! Začni warm-upem. Kolik máš dnes energie? Jak jsi spal?"

Ty: "Wall pike push up 3x8 bylo moc lehké, skoro jsem to necítil"

Claude: "To je skvělý pokrok! Zkus přejít na box pike push up - dej nohy
na lavičku/bednu výšky 40-60cm. To tě posune blíž k handstand push up,
což je na cestě k tvému cíli planche. Zkus 3x6 a řekni mi jak to bylo."

Ty: "Box pike push up 3x6 bylo lepší, ale poslední série byla těžká"

Claude: "Perfektně! To je správná intenzita. Příště dáme 3x7. Zapíšu
si box pike push up jako tvůj nový working level. Pokračuj dalším cvikem."
```

#### Po tréninku - Log a feedback
```bash
# Claude ti pomůže vytvořit strukturovaný log
# Otevři conversation a řekni "chci zalogovat dnešní trénink"
```

### 3. Týdenní review
```bash
# Každý týden zkontroluj pokrok
cat progress/weight-log.md
cat progress/calisthenics-skills.md
```

## 📁 Struktura Souborů

```
/fitness/
├── README.md                    ← Jsi zde
├── claude.md                    ← AI trenér instrukce (nečti, je to pro Claude)
├── onboarding/                  ← START ZDE při prvním použití
├── profile/                     ← Tvůj profil, cíle, omezení
├── training-logs/               ← Denní logy tréninků
├── training-plans/              ← Týdenní a měsíční plány
├── progress/                    ← Tracking pokroku (váha, síla, skills)
├── sleep/                       ← Screenshoty spánku
├── nutrition/                   ← Nepovinné poznámky o jídle
├── knowledge-base/              ← Reference materiály
└── templates/                   ← Šablony pro logy a plány
```

## 💡 Jak Komunikovat s AI Trenérem

### Real-time během tréninku:
- "Právě jsem dokončil pull-ups 5x8, cítil jsem se silný"
- "Tento cvik je moc lehký, co mám dělat?"
- "Bolí mě rameno, jak upravit dnešní trénink?"
- "Jsem dnes unavený, můžeme snížit intenzitu?"

### Plánování:
- "Udělej mi plán na příští týden"
- "Chci více pracovat na front lever, jak na to?"
- "Mám zítra málo času, můžeš zkrátit trénink?"

### Analýza pokroku:
- "Jak se mi daří s úbytkem váhy?"
- "Jsem blízko muscle upu?"
- "Co mám zlepšit?"

## 📊 Co Trackovat

### Povinné (denně):
- ✅ Spánek (screenshot)
- ✅ Trénink (cviky, série, opakování, pauzy, váhy)
- ✅ Pocity během a po tréninku

### Doporučené (týdně):
- ⚖️ Váha (1x týdně, stejný den, ráno nalačno)
- 📈 Skill tests (např. max pull-ups)

### Nepovinné:
- 🍽️ Poznámky o jídle

## ⚠️ Důležité Poznámky

1. **Buď upřímný** - Pokud tě něco bolí, cvik je moc těžký nebo lehký, řekni to!
2. **Konzistence > Dokonalost** - 4 průměrné tréninky týdně > 2 perfektní
3. **Recovery je klíčové** - Sleduj kvalitu spánku, AI ti pomůže upravit intenzitu
4. **Deficit není sprint** - Zdravý pokles je 0.5-0.7kg/týden
5. **Safety first** - Při pochybnostech konzultuj s AI, nedělej cviky špatně

## 🔄 Typický Týden

**Po/St/Pá:** Kalisthenika + síla (Upper/Lower/Full body)
**Út/Čt:** Conditioning (běh, HIIT, skill practice)
**So/Ne:** Aktivní odpočinek nebo outdoor (Kleť)

Přesný plán se bude adaptivně měnit podle tvého pokroku a recovery!

## 🆘 Help

Máš-li jakékoliv otázky, prostě se zeptej Claude v conversation modu. AI trenér je tu pro tebe 24/7.

---

**Teď jdi do `onboarding/initial-assessment.md` a začni!** 🚀
