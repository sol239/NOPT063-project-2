# Informační projekt: Prezentace o architektuře softwarových systémů

Tento projekt obsahuje dvě prezentace vytvořené v systému LaTeX (třída Beamer), které shrnují téma softwarové architektury.

## Struktura projektu

*   `img/` - Adresář s obrázky použitými v prezentacích.
*   `nova_konverzace/prezentace/` - První prezentace (zdrojový kód `prezentace.tex` a bibliografie `references.bib`).
*   `shrnuti_konverzace/prezentace/` - Druhá prezentace (zdrojový kód `prezentace.tex` a bibliografie `references.bib`).
*   `pozvanky/` - Mailové pozvánky na prezentace vygenerované různými AI modely (formální a neformální verze).

## Prerekvizity

Pro sestavení prezentací do formátu PDF potřebujete mít nainstalovanou distribuci systému LaTeX.

*   **Windows:** Doporučujeme [MiKTeX](https://miktex.org/) nebo [TeX Live](https://www.tug.org/texlive/).
*   **macOS:** [MacTeX](https://www.tug.org/mactex/).
*   **Linux:** TeX Live (např. `sudo apt-get install texlive-full`).

## Jak sestavit prezentaci (převod do PDF)

Prezentace využívají BibTeX pro správu citací, proto je potřeba specifický postup kompilace.

### Možnost 1: Příkazová řádka (Terminál)

Otevřete terminál v adresáři s konkrétní prezentací (např. `nova_konverzace/prezentace/`) a spusťte následující příkazy v tomto pořadí:

1.  **První průchod LaTeXem** (vytvoří pomocné soubory):
    ```bash
    pdflatex prezentace.tex
    ```
2.  **Generování bibliografie**:
    ```bash
    biber prezentace
    ```
3.  **Druhý průchod LaTeXem** (propojí citace):
    ```bash
    pdflatex prezentace.tex
    ```
4.  **Třetí průchod LaTeXem** (pro finální zarovnání a křížové odkazy):
    ```bash
    pdflatex prezentace.tex
    ```

Po dokončení najdete ve složce soubor `prezentace.pdf`.

### Možnost 2: VS Code (Doporučeno)

Pokud používáte Visual Studio Code, doporučujeme nainstalovat rozšíření **LaTeX Workshop**.

1.  Otevřete soubor `prezentace.tex` v editoru.
2.  Otevřete panel příkazů (`Ctrl+Shift+P` nebo `F1`).
3.  Vyhledejte a spusťte příkaz `LaTeX Workshop: Build with recipe`.
4.  Rozšíření automaticky provede celou sekvenci kompilace.
5.  Pro zobrazení PDF klikněte na ikonu lupy v pravém horním rohu editoru nebo použijte příkaz `LaTeX Workshop: View LaTeX PDF`.

## Řešení problémů

*   **Chybějící obrázky:** Ujistěte se, že složka `img/` existuje v kořenovém adresáři projektu a že cesty v `.tex` souborech (např. `../../img/obrazek.png`) jsou správné.
*   **Chybějící balíčky:** Pokud vám při kompilaci chybí nějaké LaTeX balíčky (např. `beamer`, `biblatex`), MiKTeX se je obvykle pokusí nainstalovat automaticky (vyskočí dialogové okno). U TeX Live je nutné je doinstalovat přes správce balíčků.

---

## Checklist projektu

### ✅ Splněné úkoly

- ✅ **Zvolení tématu:** Architektura softwarových systémů
- ✅ **Konverzace s chatbotem:** Získání informací o tématu za pomoci AI chatbotů
- ✅ **Ověření výstupů:** Použití různých chatbotů pro cross-checking informací
- ✅ **Ruční ověření:** Kontrola správnosti informací a testování halucinací
- ✅ **Shrnutí z konverzace:** Vytvoření souvislého textu na konci původní konverzace (`shrnuti_konverzace/shrnuti.md`)
- ✅ **Shrnutí v nové konverzaci:** Vytvoření shrnutí v nové konverzaci (`nova_konverzace/shrnuti.md`)
- ✅ **Porovnání shrnutí:** Analýza rozdílů mezi oběma shrnutími
- ✅ **LaTeX prezentace:** Vytvoření prezentace v Beameru na základě shrnutí
  - Prezentace v `nova_konverzace/prezentace/prezentace.tex`
  - Prezentace v `shrnuti_konverzace/prezentace/prezentace.tex`
- ✅ **BibTeX reference:** Správa zdrojů pomocí BibTeXu (`references.bib`)
- ✅ **Generování obrázků:** Vytvoření ilustračních obrázků pomocí AI generátorů (složka `img/`)
- ✅ **Vyhledání obrázků:** Nalezení vhodných ilustračních obrázků na internetu
- ✅ **Kompilace do PDF:** Převod LaTeX zdrojového kódu do PDF formátu
- ✅ **Formální pozvánka:** Oficiální pozvánka pro Učenou společnost (`pozvanky/*/formalni.md`)
- ✅ **Neformální pozvánka:** Přátelská pozvánka pro známé (`pozvanky/*/neformalni.md`)

