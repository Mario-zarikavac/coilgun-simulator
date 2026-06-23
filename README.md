# Coilgun Simulator

Tento repozitář obsahuje MATLAB simulátor elektromagnetického děla (coilgunu). Pro dosažení vysoké přesnosti i rychlosti využívá simulátor Lookup tabulky (LUT) předgenerované ze simulací v programu QuickField.

Pracovní název CG.ani 

## Požadavky (Prerequisites)

- **MATLAB** (R2024b nebo novější)
- **QuickField** (pro úpravy magnetického modelu a generování nových LUT)

## Instalace a naklonování repozitáře

Pro získání projektu k sobě použijte příkaz `git clone`. Pokud nemáte nastavené SSH klíče, použijte HTTPS odkaz.

```bash
git clone [https://github.com/DenisKucera/coilgun-simulator.git](https://github.com/DenisKucera/coilgun-simulator.git)
cd coilgun-simulator
```

## Použití simulátoru (Usage)

Pro spuštění simulace otevřete MATLAB, nastavte jako pracovní složku kořenový adresář tohoto repozitáře a spusťte hlavní skript.

```bash
// Přidání složek projektu do cesty MATLABu
addpath(genpath('.'));

// Spuštění hlavní simulace
run('src/main.m');
```
!!!pozn. example, bude potřeba upravit!!!

## Git Workflow

Než začnete psát kód, vždy si vytvořte novou větev pojmenovanou podle toho, na čem pracujete (např. uprava-grafu, pridani-treni). Nikdy nepracujte přímo ve větvi main!

```bash
// Ujistěte se, že jste na větvi main a máte nejnovější verzi
git checkout main
git pull

// Vytvoření a přepnutí do nové větve
git checkout -b nazev-vasi-nove-vetve
```

Jakmile provedete změny v kódu, uložte je pomocí commitu. Snažte se dělat commity logické a pište k nim jasné zprávy

```bash
// Zobrazení upravených souborů
git status

// Přidání konkrétního souboru (nebo všech pomocí 'git add .')
git add src/main.m

// Vytvoření commitu s popisem změny
git commit -m "Přidán výpočet kinetické energie do main.m"
```
