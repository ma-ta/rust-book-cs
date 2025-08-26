<!--
# Contributing

We'd love your help! Thanks for caring about the book.

## Where to Edit

All edits should be made in the `src` directory.

The `nostarch` directory contains snapshots for sending edits to the publishers
of the print version. The snapshot files reflect what has been sent or not, so
they only get updated when edits are sent to No Starch. **Do not submit pull
requests changing files in the `nostarch` directory, they will be closed.**

We use [`rustfmt`][rustfmt] to apply standard formatting to Rust code in the
repo and [`dprint`][dprint] to apply standing formatting to the Markdown source
and the non-Rust code in the project.

[rustfmt]: https://github.com/rust-lang/rustfmt
[dprint]: https://dprint.dev

You will normally have `rustfmt` installed if you have a Rust toolchain
installed; if for some reason you do not have a copy of `rustfmt`, you can add
it by running the following command:
-->
# Jak přispět

Budeme rádi za vaši pomoc! Děkujeme, že vám na této knize záleží.

## Co editovat

Veškeré úpravy by měly být prováděny v adresáři `src`.

Adresář `nostarch` obsahuje snímky pro zasílání úprav vydavatelům tištěné verze.
Soubory ve složce `nostarch` odrážejí to, co již bylo odesláno, a aktualizují
se pouze při odesílání úprav do No Starch. **Neposílejte pull requesty s
úpravami souborů v adresáři `nostarch`, budou uzavřeny.**

Používáme [`rustfmt`][rustfmt] pro standardní formátování Rust kódu v repozitáři
a [`dprint`][dprint] pro formátování Markdown zdrojů a ostatního nekódového
obsahu v projektu.

[rustfmt]: https://github.com/rust-lang/rustfmt
[dprint]: https://dprint.dev

Obvykle máte `rustfmt` nainstalovaný, pokud máte nainstalovaný Rust toolchain;
pokud jej z nějakého důvodu nemáte, můžete jej přidat následujícím příkazem:

```sh
rustup component add rustfmt
```

<!--
To install `dprint`, you can run the following command:
-->
Pro instalaci `dprint` můžete spustit následující příkaz:

```sh
cargo install dprint
```

<!--
Or follow the [instructions][install-dprint] on the `dprint` website.

[install-dprint]: https://dprint.dev/install/

To format Rust code, you can run `rustfmt <path to file>`, and to format other
files, you can pass `dprint fmt <path to file>`. Many text editors also have native
support or extensions for both `rustfmt` and `dprint`.
-->
Nebo se řídit [instrukcemi][install-dprint] na webu `dprint`.

[install-dprint]: https://dprint.dev/install/

K formátování kódu v Rustu můžete spustit příkaz `rustfmt <cesta k souboru>`,
a pro formátování ostatních souborů použít `dprint fmt <cesta k souboru>`.
Mnoho textových editorů má také vestavěnou podporu nebo rozšíření pro `rustfmt`
i `dprint`.

<!--
## Checking for Fixes

The book rides the Rust release trains. Therefore, if you see a problem on
https://doc.rust-lang.org/stable/book, it may already be fixed on the `main`
branch in this repo, but the fix hasn't gone through nightly -> beta -> stable
yet. Please check the `main` branch in this repo before reporting an issue.

Looking at the history for a particular file can also give more information on
how or whether an issue has been fixed or not if you're trying to figure that
out.

Please also search open and closed issues and open and closed PRs before
reporting a new issue or opening a new PR.
-->
## Kontrola oprav

Kniha sleduje vydání Rustu podle tzv. release trains. Pokud tedy narazíte na
problém na https://doc.rust-lang.org/stable/book, může být již opraven ve větvi
`main` v tomto repozitáři, ale oprava ještě neprošla cyklem noční -> beta
-> stabilní. Před nahlášením problému prosím zkontrolujte větev `main` v tomto
repozitáři.

Prohlédnutí historie konkrétního souboru vám může také pomoci zjistit,
zda a jak byl problém vyřešen.

Před nahlášením nového problému nebo otevřením nového pull requestu prosím
vyhledejte otevřené i uzavřené issues a nové PR.

<!--
## Licensing

This repository is under the same license as Rust itself, MIT/Apache2. You
can find the full text of each license in the `LICENSE-*` files in this
repository.
-->
## Licence

Tento repozitář je pod stejnou licencí jako samotný Rust, tedy MIT/Apache2.
Plné znění obou licencí najdete v souborech `LICENSE-*` tohoto repozitáře.

<!--
## Code of Conduct

The Rust project has [a code of conduct](http://rust-lang.org/policies/code-of-conduct)
that governs all sub-projects, including this one. Please respect it!
-->
## Kodex chování

Projekt Rust má [kodex chování](http://rust-lang.org/policies/code-of-conduct),
který platí pro všechny dílčí projekty, včetně tohoto. Prosím, respektujte jej.

<!--
## Expectations

Because the book is [printed][nostarch], and because we want
to keep the online version of the book close to the print version when
possible, it may take longer than you're used to for us to address your issue
or pull request.

[nostarch]: https://nostarch.com/rust-programming-language-2nd-edition

So far, we've been doing a larger revision to coincide with [Rust Editions](https://doc.rust-lang.org/edition-guide/). Between those larger
revisions, we will only be correcting errors. If your issue or pull request
isn't strictly fixing an error, it might sit until the next time that we're
working on a large revision: expect on the order of months or years. Thank you
for your patience!
-->
## Očekávání

Protože je kniha také v [tištěné verzi][nostarch] a snažíme se, aby online verze
byla co nejblíže té papírové, může nám vyřízení vašeho issue nebo pull requestu
trvat déle, než jste zvyklí.

[nostarch]: https://nostarch.com/rust-programming-language-2nd-edition

Dosud jsme prováděli větší revize v souvislosti s
[Rust edicemi](https://doc.rust-lang.org/edition-guide/).
Mezi těmito většími revizemi opravujeme pouze chyby. Pokud vaše issue nebo
pull request není čistě opravou chyby, může čekat až do další
velké revize – počítejte s tím, že to může být otázka měsíců nebo let.
Děkujeme za vaši trpělivost!

<!--
## Help wanted

If you're looking for ways to help that don't involve large amounts of
reading or writing, check out the [open issues with the E-help-wanted
label][help-wanted]. These might be small fixes to the text, Rust code,
frontend code, or shell scripts that would help us be more efficient or
enhance the book in some way!
-->
## Pomoc vítána

Pokud hledáte způsoby, jak pomoci, které nevyžadují velké množství čtení nebo
psaní, podívejte se na [otevřené issues s označením E-help-wanted][help-wanted].
Může jít o drobné opravy textu, Rust kódu, frontendového kódu nebo shell
skriptů, které nám pomohou být efektivnější nebo nějak vylepšit knihu!

[help-wanted]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3AE-help-wanted

<!--
## Translations

We'd love help translating the book! See the [Translations] label to join in
efforts that are currently in progress. Open a new issue to start working on
a new language! We're waiting on [mdbook support] for multiple languages
before we merge any in, but feel free to start!
-->
## Překlady

## Překlady

Rádi uvítáme pomoc s překladem knihy! Podívejte se na štítek [Překlady],
abyste se zapojili do probíhajících překladatelských prací. Otevřete nový
problém (issue), pokud chcete začít pracovat na novém jazyce!
Čekáme na [podporu mdbooku] pro více jazyků, než některý z překladů začleníme,
ale klidně můžete začít hned!

[Překlady]: https://github.com/rust-lang/book/issues?q=is%3Aopen+is%3Aissue+label%3ATranslations
[mdbook support]: https://github.com/rust-lang/mdBook/issues/5
