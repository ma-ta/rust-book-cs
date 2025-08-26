<!--
# The Rust Programming Language
-->
# Programovací jazyk Rust

![Build Status](https://github.com/rust-lang/book/workflows/CI/badge.svg)

<!--
This repository contains the source of "The Rust Programming Language" book.

[The book is available in dead-tree form from No Starch Press][nostarch].
-->
Tento repozitář obsahuje zdrojové soubory knihy o programovacím jazyce Rust
„The Rust Programming Language“.

[Kniha je k dispozici v tištěné podobě od vydavatelství No Starch Press][nostarch].

[nostarch]: https://nostarch.com/rust-programming-language-2nd-edition

<!--
You can also read the book for free online. Please see the book as shipped with
the latest [stable], [beta], or [nightly] Rust releases. Be aware that issues
in those versions may have been fixed in this repository already, as those
releases are updated less frequently.
-->
Knihu si můžete také přečíst zdarma online. Podívejte se na verzi knihy,
která odpovídá nejnovějším [stabilním], [beta] nebo [nočním] vydáním Rustu.
Mějte na paměti, že problémy v těchto verzích mohly být v tomto repozitáři
již opraveny, protože tato vydání jsou aktualizována méně často.

[stabilním]: https://doc.rust-lang.org/stable/book/
[beta]: https://doc.rust-lang.org/beta/book/
[nočním]: https://doc.rust-lang.org/nightly/book/

<!--
See the [releases] to download just the code of all the code listings that
appear in the book.
-->
Podívejte se na [releases], kde si můžete stáhnout pouze zdrojové kódy
všech ukázek, které se v knize objevují.

[releases]: https://github.com/rust-lang/book/releases

<!--
## Requirements

Building the book requires [mdBook], ideally the same version that
rust-lang/rust uses in [this file][rust-mdbook]. To get it:
-->
## Požadavky

Pro sestavení knihy je potřeba [mdBook], ideálně ve stejné verzi, jakou používá
rust-lang/rust v [tomto souboru][rust-mdbook]. Chcete-li jej získat:

[mdBook]: https://github.com/rust-lang/mdBook
[rust-mdbook]: https://github.com/rust-lang/rust/blob/master/src/tools/rustbook/Cargo.toml

```bash
$ cargo install mdbook --locked --version <version_num>
```

<!--
The book also uses two mdbook plugins which are part of this repository. If you
do not install them, you will see warnings when building and the output will not
look right, but you _will_ still be able to build the book. To use the plugins,
you should run:
-->
Kniha také používá dva pluginy pro mdbook, které jsou součástí tohoto
repozitáře. Pokud je nenainstalujete, při sestavování se zobrazí varování
a výstup nebude vypadat správně, ale knihu přesto _budete schopni_ sestavit.
Pro použití těchto pluginů byste měli spustit:

```bash
$ cargo install --locked --path packages/mdbook-trpl --force
```

<!--
## Building

To build the book, type:
-->
## Sestavení

Pro sestavení knihy zadejte:

```bash
$ mdbook build
```

<!--
The output will be in the `book` subdirectory. To check it out, open it in
your web browser.
-->
Výstup bude ve podadresáři `book`. Pro jeho zobrazení jej otevřete ve svém
webovém prohlížeči.

_Firefox:_

```bash
$ firefox book/index.html                       # Linux
$ open -a "Firefox" book/index.html             # OS X
$ Start-Process "firefox.exe" .\book\index.html # Windows (PowerShell)
$ start firefox.exe .\book\index.html           # Windows (Cmd)
```

_Chrome:_

```bash
$ google-chrome book/index.html                 # Linux
$ open -a "Google Chrome" book/index.html       # OS X
$ Start-Process "chrome.exe" .\book\index.html  # Windows (PowerShell)
$ start chrome.exe .\book\index.html            # Windows (Cmd)
```

<!--
To run the tests:
-->
Pro spuštění testů:

```bash
$ cd packages/trpl
$ mdbook test --library-path packages/trpl/target/debug/deps
```

<!--
## Contributing

We'd love your help! Please see [CONTRIBUTING.md][contrib] to learn about the
kinds of contributions we're looking for.

[contrib]: https://github.com/rust-lang/book/blob/main/CONTRIBUTING.md

Because the book is [printed][nostarch], and because we want
to keep the online version of the book close to the print version when
possible, it may take longer than you're used to for us to address your issue
or pull request.

So far, we've been doing a larger revision to coincide with [Rust Editions](https://doc.rust-lang.org/edition-guide/). Between those larger
revisions, we will only be correcting errors. If your issue or pull request
isn't strictly fixing an error, it might sit until the next time that we're
working on a large revision: expect on the order of months or years. Thank you
for your patience!
-->
## Jak přispět

Rádi uvítáme vaši pomoc! Podívejte se na [CONTRIBUTING.md][contrib], abyste
se dozvěděli, jaké typy výpomoci hledáme.

[contrib]: https://github.com/rust-lang/book/blob/main/CONTRIBUTING.md

Protože je kniha také v [tištěné verzi][nostarch] a snažíme se, aby online verze
byla co nejblíže té papírové, může nám vyřízení vašeho issue nebo pull requestu
trvat déle, než jste zvyklí.

Dosud jsme prováděli větší revize v souvislosti s
[Rust edicemi](https://doc.rust-lang.org/edition-guide/).
Mezi těmito většími revizemi opravujeme pouze chyby. Pokud vaše issue nebo
pull request není čistě opravou chyby, může čekat až do další
velké revize – počítejte s tím, že to může být otázka měsíců nebo let.
Děkujeme za vaši trpělivost!

<!--
### Translations

We'd love help translating the book! See the [Translations] label to join in
efforts that are currently in progress. Open a new issue to start working on
a new language! We're waiting on [mdbook support] for multiple languages
before we merge any in, but feel free to start!
-->
### Překlady

Rádi uvítáme pomoc s překladem knihy! Podívejte se na štítek [Překlady],
abyste se zapojili do probíhajících překladatelských prací. Otevřete nový
problém (issue), pokud chcete začít pracovat na novém jazyce!
Čekáme na [podporu mdbooku] pro více jazyků, než některý z překladů začleníme,
ale klidně můžete začít hned!

[Překlady]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3ATranslations
[podporu mdbooku]: https://github.com/rust-lang/mdBook/issues/5

<!--
## Spellchecking

To scan source files for spelling errors, you can use the `spellcheck.sh`
script available in the `ci` directory. It needs a dictionary of valid words,
which is provided in `ci/dictionary.txt`. If the script produces a false
positive (say, you used the word `BTreeMap` which the script considers invalid),
you need to add this word to `ci/dictionary.txt` (keep the sorted order for
consistency).
-->
## Kontrola pravopisu

Pro kontrolu zdrojových souborů na pravopisné chyby můžete použít skript
`spellcheck.sh`, který je k dispozici v adresáři `ci`. Skript potřebuje
slovník platných slov, který je poskytnut v `ci/dictionary.txt`.
Pokud skript vykáže falešně pozitivní výsledek (například použijete slovo
`BTreeMap`, které skript považuje za neplatné), je třeba toto slovo přidat
do `ci/dictionary.txt` (dodržujte řazení slov pro konzistenci).