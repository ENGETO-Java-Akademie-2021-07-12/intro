<p align="center">
  <img src="https://engeto.cz/wp-content/uploads/2019/01/engeto-square.png" width="200" height="200">
</p>

# Příprava na první lekci Javy, aneb každý malíř potřebuje své plátno

Před tím, než se spolu na první lekci ponoříme do tajů Javy a&nbsp;vytvoříme si první program, máme tu pro Tebe první quest &mdash; připravit si své „malířské plátno“, tedy v&nbsp;našem případě vývojové prostředí.

Co budeme potřebovat? Prozatím nám budou stačit: JDK, IntelliJ IDEA a&nbsp;účet na GitHubu.

## JDK

JDK, neboli Java Development Kit je balíček základních nástrojů pro vývoj v&nbsp;Javě, který si potřebuješ stáhnout a nainstalovat.

Jdi na stránku: https://www.oracle.com/java/technologies/javase-jdk11-downloads.html a zde si stáhni instalační balíček podle toho, jaký máš operační systém (po zvolení instalačního balíčku budeš přesměrován na stránky Oracle, kde si budeš muset vytvořit účet a/nebo se přihlásit).

- v&nbsp;případě, že máš Windows, zvol: <b>Windows x64 Installer</b> a pokračuj kroky popsanými v části [<b>Instalace JDK ve Windows</b>](#instalace-jdk-ve-windows)

- v případě, že máš MAC OS, zvol: <b>macOS Installer</b> a pokračujte kroky popsanými v&nbsp;části [<b>Instalace JDK v MAC OS</b>](#instalace-jdk-v-mac-os)

- v případě, že máš Fedoru, případně jinou linuxovou distribuci založenou na Red Hatu, zvol: <b>Linux RPM Package</b> a pokračuj kroky popsanými v části [<b>Instalace JDK v&nbsp;Red Hat-based distribuci</b>](#instalace-jdk-v-red-hat-based-distribuci)

- v případě, že máš Ubuntu, případně jinou linuxovou distribuci založenou na Debianu, zvol: <b>Linux Debian Package</b> a pokračujte kroky popsanými v&nbsp;části [<b>Instalace JDK v Debian-based distribuci</b>](#instalace-jdk-v-debian-based-distribuci)

### Instalace JDK ve Windows

- ve stažených souborech klikni pravým tlačítkem na stažený instalační balíček a&nbsp;zvol „Spustit jako administrátor“

- v instalačním okně pak zbývá zmáčknout třikrát tlačítko <b>Next</b>, čímž nejrve potvrdíš, co instaluješ, následně budeš mít možnost zvolit dodatečné části k&nbsp;naistalování - tady chceš nechat defaultní nastavení a můžeš tedy pokračovat zase stiskem tlačítka <b>Next</b>, nakonec máš možnost zvolit, do jaké složky se bude instalovat - zde opět není potřeba nic měnit a můžeš opět pokračovat stiskem tlačítka <b>Next</b>, tím se začne instalovat a po dokončení už stačí jen zavřít okno tlačítkem <b>Close</b>

### Instalace JDK v MAC OS
 
 - v <b>Downloads</b>, případně v&nbsp;prohlížeči souborů dvakrát klikni na stažený instalační balíček s koncovkou <i>.dmg</i> - zobrazí se Ti okno <b>Finder</b> a v&nbsp;něm soubor s&nbsp;koncovkou <i>.pkg</i>
 
 - dvouklikem klikni na soubor s koncovkou <i>.pkg</i>, čímž zahájíš instalaci - zobrazí se Ti okno <b>Introduction</b>
 
 - klikni na tlačítko <b>Continue</b> - objeví se okno <b>Installation Type</b>
 
 - klikni na tlačítko <b>Install</b> - zobrazí se Ti okno se zprávou: „Installer is trying to install new software. Enter your password to allow this.“
 
 - zadej administrátorské jméno a heslo a klikni na tlačítko <b>Install Software</b>, nyní už zbývá jen počkat a následně odkliknout potvrzovaní okno o úspěšné instalaci

### Instalace JDK v Red Hat-based distribuci

- v konzoli se přepni do adresáře, do kterého chceš JDK nainstalovat a následně tam přesuň stažený instalační soubor s koncovkou <i>.tar.gz</i>

- samotnou instalaci pak provedeš příkazem <i>tar zxvf jmeno_stazeneho_instalacniho_balicku.tar.gz</i>

### Instalace JDK v Debian-based distribuci

- ujisti se, že jsi přihlášen(a) jako root — v&nbsp;konzoli zadejte příkaz <i>su</i> a následně zadejte heslo superusera

- samotnou instalaci provedeš příkazem <i>rpm -ivh jmeno_stazeneho_instalacniho_balicku.rpm</i>

## IntelliJ IDEA

Tohle bude naše vývojové prostředí ve kterém budeme psát (a testovat) samotný kód.

Potřebujeme si je stáhnout, nainstalovat a nastavit.

Jdi na stránku: https://www.jetbrains.com/idea/download/

Zde si podle svého operačního systému (Windows/MAC OS/Linux) zvol správnou verzi a stáhni si edici nazvanou <b>Community</b>. Pak pokračuj pomocí níže uvedeného návodu pro svůj operační systém

### Instalace IntelliJ IDEA ve Windows

- dvouklikem klikni na stažený instalační soubor s koncovkou <i>.exe</i> - otevře se Ti okno, které Tě provede instalací

- základní nastavení nepotřebujeme měnit, takže nyní stačí 4× stiknout tlačítko <b>Next</b> a v okně s nápisem „Completing IntelliJ IDEA setup“, informujícím o úspěšně dokončené instalaci, zruš možnost „Run IntelliJ IDEA“ a klini na <b>Finish</b>

### Instalace IntelliJ IDEA v MAC OS

- otevři si instalační soubor s koncovkou <i>.dmg</i>, který sis stáhl(a) a přesuň v okně, které se Ti otevře, IntelliJ IDEA do složky „Applications“

### Instalace IntelliJ IDEA v&nbsp;Linuxu

- Stáhni si instalační balíček ze stránek: https://www.jetbrains.com/idea/download/

- Zvol verzi Community Edition pro Linux.

- Rozbal stažený soubor a&nbsp;spusť soubor `idea.sh` z&nbsp;adresáře `bin`.

- Po spuštění nastav JDK: Klikneme na _Configure... → Structure for New Projects_ a&nbsp;vybereme ze seznamu _Detected SDKs → /usr/java/latest_.

## Podrobnější návod

Podrobnější návod najdeš [v&nbsp;kurzu Java#1](https://engeto.com/cs/kurz/java-1-uvod-do-programovani/studium/m_TDBn4hQyyJ7Hp2uFS5Sw/zaciname-s-javou/priprava-prostredi/stazeni-oracle-jdk).

---

## GitHub

Zatím stačí, když si na GitHubu vytvoříš účet:

- Jdi na stránku: https://github.com/

- Zde vyplň uživatelské jméno, e-mail a&nbsp;heslo a&nbsp;klikni na tlačítko <b>Sign up for GitHub</b>

- Vytvořené uživatelské jméno pošli lektorovi přes Slack. Zpřístupní ti obsah dalších lekcí.


---

[Zpět na přehled akademie](https://github.com/ENGETO-Java-Akademie-2021-07-12/intro)