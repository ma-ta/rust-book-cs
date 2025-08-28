<!--
## Appendix A: Keywords

The following list contains keywords that are reserved for current or future
use by the Rust language. As such, they cannot be used as identifiers (except
as raw identifiers as we’ll discuss in the “[Raw
Identifiers][raw-identifiers]” section). Identifiers are names
of functions, variables, parameters, struct fields, modules, crates, constants,
macros, static values, attributes, types, traits, or lifetimes.

[raw-identifiers]: #raw-identifiers
-->
## Dodatek A: Klíčová slova

Následující seznam obsahuje klíčová slova, která jsou v jazyce Rust
rezervována pro současné nebo budoucí použití. Proto je nelze použít jako
identifikátory (kromě tzv. *raw identifikátorů*, o kterých budeme mluvit v
části „[Raw identifikátory][raw-identifiers]<!-- ignore -->“).
Identifikátory jsou názvy funkcí, proměnných, parametrů, položek ve
strukturách, modulů, crate balíčků, konstant, maker, statických hodnot,
atributů, typů, traitů nebo lifetimů.

[raw-identifiers]: #raw-identifikátory

<!--
### Keywords Currently in Use

The following is a list of keywords currently in use, with their functionality
described.
-->
### Klíčová slova využívaná v současnosti

Následuje seznam klíčových slov, která se v současnosti používají, spolu
s popisem jejich funkce.

<!--
- `as` - perform primitive casting, disambiguate the specific trait containing
  an item, or rename items in `use` statements
- `async` - return a `Future` instead of blocking the current thread
- `await` - suspend execution until the result of a `Future` is ready
- `break` - exit a loop immediately
- `const` - define constant items or constant raw pointers
- `continue` - continue to the next loop iteration
- `crate` - in a module path, refers to the crate root
- `dyn` - dynamic dispatch to a trait object
- `else` - fallback for `if` and `if let` control flow constructs
- `enum` - define an enumeration
- `extern` - link an external function or variable
- `false` - Boolean false literal
- `fn` - define a function or the function pointer type
- `for` - loop over items from an iterator, implement a trait, or specify a
  higher-ranked lifetime
- `if` - branch based on the result of a conditional expression
- `impl` - implement inherent or trait functionality
- `in` - part of `for` loop syntax
- `let` - bind a variable
- `loop` - loop unconditionally
- `match` - match a value to patterns
- `mod` - define a module
- `move` - make a closure take ownership of all its captures
- `mut` - denote mutability in references, raw pointers, or pattern bindings
- `pub` - denote public visibility in struct fields, `impl` blocks, or modules
- `ref` - bind by reference
- `return` - return from function
- `Self` - a type alias for the type we are defining or implementing
- `self` - method subject or current module
- `static` - global variable or lifetime lasting the entire program execution
- `struct` - define a structure
- `super` - parent module of the current module
- `trait` - define a trait
- `true` - Boolean true literal
- `type` - define a type alias or associated type
- `union` - define a [union][union]; is only a keyword when used
  in a union declaration
- `unsafe` - denote unsafe code, functions, traits, or implementations
- `use` - bring symbols into scope; specify precise captures for generic and
  lifetime bounds
- `where` - denote clauses that constrain a type
- `while` - loop conditionally based on the result of an expression
-->
- `as` - provádí primitivní přetypování, určuje konkrétní trait obsahující
  prvek, nebo přejmenovává položky v `use` příkazech
- `async` - vrací `Future` namísto blokování aktuálního vlákna
- `await` - pozastaví vykonávání, dokud není výsledek `Future` připraven
- `break` - okamžitě ukončí cyklus
- `const` - definuje konstanty nebo konstantní raw ukazatele
- `continue` - přeskočí na další iteraci cyklu
- `crate` - v cestě modulu odkazuje na crate root
- `dyn` - dynamické volání trait objektu
- `else` - větev příkazu `if` a `if let`
- `enum` - definuje výčtový typ
- `extern` - propojuje externí funkci nebo proměnnou
- `false` - literál logické hodnoty nepravda
- `fn` - definuje funkci nebo typ ukazatele na funkci
- `for` - iteruje přes položky z iterátoru, implementuje trait nebo určuje
  higher-ranked lifetime
- `if` - větvení podle výsledku podmíněného výrazu
- `impl` - implementuje vlastní nebo traitovou funkcionalitu
- `in` - součást syntaxe `for` cyklu
- `let` - definuje proměnnou
- `loop` - cyklus bez podmínky (nekonečný)
- `match` - porovnává hodnotu se vzory (pattern matching)
- `mod` - definuje modul
- `move` - způsobí, že uzávěr (closure) převezme vlastnictví všech
  zachycených hodnot
- `mut` - označuje mutabilitu v referencích, raw ukazatelích
  nebo pattern bindings
- `pub` - označuje veřejnou viditelnost položek ve strukturách, `impl` blocích
  nebo modulech
- `ref` - prováže odkazem
- `return` - ukončí funkci (a vrátí hodnotu)
- `Self` - typový alias pro typ, který právě definujeme nebo implementujeme
- `self` - objekt metody nebo daného modulu
- `static` - globální proměnná nebo lifetime trvající po celou dobu běhu
  programu
- `struct` - definuje strukturu
- `super` - nadřazený modul aktuálního modulu
- `trait` - definuje trait (rozhraní / vlastnost)
- `true` - literál logické hodnoty pravda
- `type` - definuje typový alias nebo asociovaný typ
- `union` - definuje [union][union]<!-- ignore -->; je klíčovým slovem pouze
  v deklaraci unionu
- `unsafe` - označuje nezabezpečený (unsafe) kód, funkce, traity
  nebo implementace
- `use` - zavádí symboly do aktuálního oboru viditelnosti; umožňuje přesně
  určit zachycení pro generické parametry a lifetime (omezení životnosti)
- `where` - určuje podmínky (klauzule), které omezují typ
- `while` - podmíněný cyklus založený na výsledku výrazu

[union]: ../reference/items/unions.html

<!--
### Keywords Reserved for Future Use

The following keywords do not yet have any functionality but are reserved by
Rust for potential future use.
-->
### Klíčová slova rezervovaná pro budoucí použití

Následující klíčová slova zatím nemají žádnou funkci, ale jsou v Rustu
rezervována pro možné budoucí využití.

- `abstract`
- `become`
- `box`
- `do`
- `final`
- `gen`
- `macro`
- `override`
- `priv`
- `try`
- `typeof`
- `unsized`
- `virtual`
- `yield`

<!--
### Raw identifikátory

_Raw identifiers_ are the syntax that lets you use keywords where they wouldn’t
normally be allowed. You use a raw identifier by prefixing a keyword with `r#`.

For example, `match` is a keyword. If you try to compile the following function
that uses `match` as its name:
-->
### Raw identifikátory

_Raw identifikátory_ jsou syntaxe, která vám umožňuje použít klíčová slova tam,
kde by normálně nebyla povolena.
Raw identifikátor použijete tak, že před klíčové slovo napíšete `r#`.

Například `match` je klíčové slovo. Pokud se pokusíte zkompilovat následující
funkci, která používá `match` jako své jméno:

<span class="filename">Filename: src/main.rs</span>

```rust,ignore,does_not_compile
fn match(needle: &str, haystack: &str) -> bool {
    haystack.contains(needle)
}
```

<!--
you’ll get this error:
-->
dostanete tuto chybu:

```text
error: expected identifier, found keyword `match`
 --> src/main.rs:4:4
  |
4 | fn match(needle: &str, haystack: &str) -> bool {
  |    ^^^^^ expected identifier, found keyword
```

<!--
The error shows that you can’t use the keyword `match` as the function
identifier. To use `match` as a function name, you need to use the raw
identifier syntax, like this:
-->
Chyba ukazuje, že nelze použít klíčové slovo `match` jako identifikátor
funkce. Chcete-li použít `match` jako název funkce, musíte použít syntaxi
raw identifikátoru, například takto:

<span class="filename">Filename: src/main.rs</span>

```rust
fn r#match(needle: &str, haystack: &str) -> bool {
    haystack.contains(needle)
}

fn main() {
    assert!(r#match("foo", "foobar"));
}
```

<!--
This code will compile without any errors. Note the `r#` prefix on the function
name in its definition as well as where the function is called in `main`.

Raw identifiers allow you to use any word you choose as an identifier, even if
that word happens to be a reserved keyword. This gives us more freedom to choose
identifier names, as well as lets us integrate with programs written in a
language where these words aren’t keywords. In addition, raw identifiers allow
you to use libraries written in a different Rust edition than your crate uses.
For example, `try` isn’t a keyword in the 2015 edition but is in the 2018, 2021,
and 2024 editions. If you depend on a library that is written using the 2015
edition and has a `try` function, you’ll need to use the raw identifier syntax,
`r#try` in this case, to call that function from your code on later editions.
See [Appendix E][appendix-e] for more information on editions.
-->
Tento kód se zkompiluje bez chyb. Povšimněte si prefixu `r#` jak u názvu funkce
při její definici, tak při volání ve funkci `main`.

Raw identifikátory vám umožňují použít libovolné slovo jako identifikátor,
i když se jedná o rezervované klíčové slovo. To nám dává větší volnost při
volbě názvů identifikátorů a zároveň umožňuje integraci s programy napsanými
v jazyce, v němž tato slova nejsou klíčovými slovy. Krom toho raw
identifikátory umožňují používat knihovny napsané v jiné edici Rustu,
než kterou používá váš crate. Například `try` není klíčové slovo v edici 2015,
ale je jím v edicích 2018, 2021 a 2024. Pokud závisíte na knihovně napsané
v edici 2015, která má funkci `try`, budete muset použít syntaxi
raw identifikátoru, v tomto případě `r#try`, abyste tuto funkci mohli volat
z vašeho kódu v novějších edicích. Více informací o edicích naleznete
v [Dodatku E][appendix-e]<!-- ignore -->.

[appendix-e]: appendix-05-editions.html
