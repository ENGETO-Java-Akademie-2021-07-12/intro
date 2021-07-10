<p align="center">
  <img src="https://engeto.cz/wp-content/uploads/2019/01/engeto-square.png" width="200" height="200">
</p>

# Příprava na první lekci Javy, aneb každý malíř potřebuje své plátno

Před tím, než se spolu na první lekci ponoříme do tajů Javy a vytvoříme si první program, tu pro Vás mám drobný quest - připravit si své "malířské plátno", tedy v našem případě vývojové prostředí.
Co budeme potřebovat? Prozatím nám budou stačit tyto tři věci: JDK, IntelliJ IDEA a GitHub

## JDK

JDK, neboli Java Development Kit je balíček základních nástrojů pro vývoj v Javě, který si potřebujeme stáhnout a nainstalovat.

Jděte na stránku: https://www.oracle.com/java/technologies/javase-jdk11-downloads.html a zde si stáhněte instalační balíček podle toho, jaký máte operační systém (po zvolení instalačního balíčku budete přesměrováni na stránky Oracle, kde si budete muset muset vytvořit účet a/nebo se přihlásit).

- v případě, že máte Windows, zvolte: <b>Windows x64 Installer</b> a pokračujte kroky popsanými v části [<b>Instalace JDK ve Windows</b>](#instalace-jdk-ve-windows)

- v případě, že máte MAC OS, zvolte: <b>macOS Installer</b> a pokračujte kroky popsanými v části [<b>Instalace JDK v MAC OS</b>](#instalace-jdk-v-mac-os)

- v případě, že máte Fedoru, případně jinou Linuxovou distribuci založenou na Red Hatu, zvolte: <b>Linux RPM Package</b> a pokračujte kroky popsanými v části [<b>Instalace JDK v Red Hat-based distribuci</b>](#instalace-jdk-v-red-hat-based-distribuci)

- v případě, že máte Ubuntu, případně jinou Linuxovou distribuci založenou na Debianu, zvolte: <b>Linux Debian Package</b> a pokračujte kroky popsanými v části [<b>Instalace JDK v Debian-based distribuci</b>](#instalace-jdk-v-debian-based-distribuci)

### Instalace JDK ve Windows

- ve stažených souborech kliknete pravým tlačítkem na stažený instalační balíček a zvolíte spustit jako administrátor

- v instalačním okně pak zbývá zmáčknout třikrát tlačítko <b>Next</b>, čímž nejrve potvrdíte, co instalujete, následně budete mít možnost zvolit dodatečné části k naistalování - tady chcete nechat defaultní nastavení a můžete tedy pokračovat zase stiskem tlačítka <b>Next</b>, nakonec máte možnost zvolit, do jaké složky se bude instalovat - zde opět není potřeba nic měnit a můžete opět pokračovat stiskem tlačítka <b>Next</b>, tím se začne instalovat a po dokončení už stačí jen zavřít okno tlačítkem <b>Close</b>

### Instalace JDK v MAC OS
 
 - v <b>Downloads</b>, případně ve prohlížeči souborů dvakrát klikněte na stažený instalační balíček s koncovkou <i>.dmg</i> - zobrazí se Vám okno <b>Finder</b> a v něm soubor s koncovkou <i>.pkg</i>
 
 - dvouklikem klikněte na soubor s koncovkou <i>.pkg</i>, čímž zahájíte instalaci - zobrazí se Vám okno <b>Introduction</b>
 
 - klikněte na tlačítko <b>Continue</b> - objeví se okno <b>Installation Type</b>
 
 - klikněte na tlačítko <b>Install</b> - zobrazí se Vám okno se zprávou: "Installer is trying to install new software. Enter your password to allow this."
 
 - zadejte administrátorské jméno a heslo a klikněte na tlačítko <b>Install Software</b>, nyní už zbývá jen počkat a následně odkliknout potvrzovaní okno o úspěšné instalaci

### Instalace JDK v Red Hat-based distribuci

- v konzoli se přepněte do adresáře, do kterého chcete JDK nainstalovat a následně tam přesuňte stažený instalační soubor s koncovkou <i>.tar.gz</i>

- samotnou instalaci pak provedete příkazem <i>tar zxvf jmeno_stazeneho_instalacniho_balicku.tar.gz</i>

### Instalace JDK v Debian-based distribuci

- ujistěte se, že jste přihlášeni jako root - v konzoli zadejte příkaz <i>su</i> a následně zadejte heslo superusera

- samotnou instalaci provedete příkazem <i>rpm -ivh jmeno_stazeneho_instalacniho_balicku.rpm</i>

## IntelliJ IDEA

Tohle bude naše vývojové prostředí ve kterém budeme psát (a testovat) samotný kód.

Potřebujeme si je stáhnout, nainstalovat a nastavit.

Jděte na stránku: https://www.jetbrains.com/idea/download/

Zde si podle vašeho operačního systému (Windows/MAC OS/Linux) zvolte správnou verzi a stáhněte si edici nazvanou <b>Community</b> a pokračujte pomocí níže uvedeného návodu pro váš operační systém

### Instalace IntelliJ IDEA ve Windows

- dvouklikem klikněte na stažený instalační soubor s koncovkou <i>.exe</i> - otevře se Vám okno, které Vás provede instalací

- základní nastavení nepotřebujeme měnit, takže nyní stačí 4* stiknout tlačítko <b>Next</b> a v okně s nápisem "Completing IntelliJ IDEA setup" informujícím o úspěšně dokončené instalaci odvyberte možnost "Run IntelliJ IDEA" a kliněte na <b>Finish</b>

### Instalace IntelliJ IDEA v MAC OS

-  otevřete si instalační soubor s koncovkou <i>.dmg</i>, který jste si stáhli a přesuňte v okně, které se Vám otevře, IntelliJ IDEA do složky "Applications"

### Instalace IntelliJ IDEA v&nbsp;Linuxu

- Stáhneme si instalační balíček ze stránek: https://www.jetbrains.com/idea/download/

- Zvolíme verzi Community Edition pro Linux.

- Rozbal stažený soubor a&nbsp;spusť soubor `idea.sh` z&nbsp;adresáře `bin`.

- Po spuštění nastav JDK: Klikneme na _Configure... → Structure for New Projects_ a&nbsp;vybereme ze seznamu _Detected SDKs → /usr/java/latest_.

## Podrobnější návod

Podrobnější návod najdeš [v&nbsp;kurzu Java#1](https://engeto.com/cs/kurz/java-1-uvod-do-programovani/studium/m_TDBn4hQyyJ7Hp2uFS5Sw/zaciname-s-javou/priprava-prostredi/stazeni-oracle-jdk).

---

## GitHub

Zde nám zatím stačí si vytvořit účet.

- Jděte na stránku: https://github.com/

- Zde vyplňte uživatelské jméno, email a heslo a klikněte na tlačítko <b>Sign up for GitHub</b>

- Vytvořené uživatelské jméno pošli lektorovi přes Slack. Zpřístupní ti obsah dalších lekcí.