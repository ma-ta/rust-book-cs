<!--
# Foreword

It wasn’t always so clear, but the Rust programming language is fundamentally
about _empowerment_: no matter what kind of code you are writing now, Rust
empowers you to reach farther, to program with confidence in a wider variety of
domains than you did before.

Take, for example, “systems-level” work that deals with low-level details of
memory management, data representation, and concurrency. Traditionally, this
realm of programming is seen as arcane, accessible only to a select few who
have devoted the necessary years learning to avoid its infamous pitfalls. And
even those who practice it do so with caution, lest their code be open to
exploits, crashes, or corruption.
-->
# Předmluva

Nebývalo to vždy tak jasné, ale programovací jazyk Rust vám obecně rozšiřuje
schopnosti: bez ohledu na to, jaký typ kódu právě píšete, Rust vám umožňuje jít
dál, programovat s jistotou v širší škále oblastí než dříve.

Vezměme si například „systémové“ programování, které se potýká s nízkoúrovňovými
detaily správy paměti, reprezentací dat a paralelismem. Tradičně je tato oblast
považována za tajemnou, přístupnou jen hrstce těch, kteří věnovali roky studiu,
aby se vyhnuli jejím pověstným nástrahám. A i ti, kteří se jí věnují, tak činí
s opatrností, aby jejich kód nebyl náchylný k útokům, pádům nebo poškození dat.

<!--
Rust breaks down these barriers by eliminating the old pitfalls and providing a
friendly, polished set of tools to help you along the way. Programmers who need
to “dip down” into lower-level control can do so with Rust, without taking on
the customary risk of crashes or security holes, and without having to learn
the fine points of a fickle toolchain. Better yet, the language is designed to
guide you naturally towards reliable code that is efficient in terms of speed
and memory usage.

Programmers who are already working with low-level code can use Rust to raise
their ambitions. For example, introducing parallelism in Rust is a relatively
low-risk operation: the compiler will catch the classical mistakes for you. And
you can tackle more aggressive optimizations in your code with the confidence
that you won’t accidentally introduce crashes or vulnerabilities.
-->
Rust odstraňuje tyto bariéry tím, že eliminuje staré nástrahy a nabízí
přívětivou, propracovanou sadu nástrojů, které vám na cestě pomohou.
Programátoři, kteří potřebují „sestoupit“ k nízkoúrovňovým oblastem, tak mohou
s Rustem učinit bez obvyklého rizika pádů nebo bezpečnostních děr, aniž by
museli znát všechny detaily rozličných nástrojů. Jazyk je navíc navržen tak,
aby vás přirozeně vedl k spolehlivému kódu, který je efektivní z hlediska
rychlosti i spotřeby paměti.

Programátoři, kteří již s nízkoúrovňovým kódem pracují, mohou díky Rustu zvýšit
své ambice. Například zavedení paralelismu v Rustu je poměrně bezpečná operace:
překladač za vás odhalí klasické chyby. Můžete se tak pustit do agresivnějších
optimalizací s jistotou, že omylem nezpůsobíte pády nebo bezpečnostní
zranitelnosti.

<!--
But Rust isn’t limited to low-level systems programming. It’s expressive and
ergonomic enough to make CLI apps, web servers, and many other kinds of code
quite pleasant to write — you’ll find simple examples of both later in the
book. Working with Rust allows you to build skills that transfer from one
domain to another; you can learn Rust by writing a web app, then apply those
same skills to target your Raspberry Pi.

This book fully embraces the potential of Rust to empower its users. It’s a
friendly and approachable text intended to help you level up not just your
knowledge of Rust, but also your reach and confidence as a programmer in
general. So dive in, get ready to learn—and welcome to the Rust community!
-->
Rust však není omezen jen na nízkoúrovňové systémové programování. Je
dostatečně expresivní a ergonomický, aby bylo příjemné psát například CLI
aplikace, webové servery a mnoho dalších typů kódu — jednoduché příklady z
obou oblastí najdete dále v této knize. Práce s Rustem vám umožní získat
dovednosti, které snadno využijete v různých oblastech; můžete se Rust naučit
při psaní webové aplikace a stejné znalosti pak použít třeba pro Raspberry Pi.

Tato kniha plně využívá potenciál Rustu činit ze svých uživatelů schopnější
programátory. Je přátelským a přístupným textem, který vám pomůže nejen zvýšit
znalosti o Rustu, ale také vaše možnosti a sebevědomí jako programátora obecně.
Pusťte se do práce, připravte se učit — a vítejte v komunitě Rustu!

<!--
— Nicholas Matsakis and Aaron Turon
-->
— Nicholas Matsakis a Aaron Turon
