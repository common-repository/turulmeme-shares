=== Turulmeme shares ===
Contributors: rrd
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=1880117
Tags: comments, Google Reader, turulmeme
Requires at least: 2.0.2
Tested up to: 2.7.1
Stable tag: 0.5.5

A bejegyzéseidben megjelenjenek azok a hozzászólások amelyeket a Turulmemén lévő userek adtak hozzá.

== Description ==

A plugin segítségével a bejegyzéseink alatt megjeleníthetjük, hogy kik osztották meg a bejegyzést a Turulmemén és milyen hozzászólásokat írtak hozzá.

Az admin oldalon együtt tudjuk látni, hogy melyik bejegyzésünkhöz kik és mit szóltak hozzá, valamint lehetőségünk van a hozzászólások moderálására.

== Installation ==

1. Töltsd le a Turulmeme shares plugint és csomagold ki.
2. A kicsomagolt könyvtárat másold fel a blogod `/wp-content/plugins` könyvtárába
3. Válaszd ki a sablonszerkesztés menüpontot és a sablonod bejegyzés (single.php) fájljába szúrd be a következő sort: `<?php if(function_exists('turulmeme_shares')){	turulmeme_shares('<h3>Google Reader hozzászólások</h3>'); } ?>`
4. Végül a bővítmények (plugins) oldalon kapcsold be a plugint.


== Frequently Asked Questions ==

= Hogyan módosíthatom a lista kinézetét? =

A lista kinézete egyszerűen módosítható a plugin könyvtárban található CSS file módosításával.

= Mit jelent a moderálás? =

Mivel ezeket a hozzászólásokat a felhasználók a saját Google Reader fiókjukban teszik eg valójában nem tudjuk őket moderálni. A moderálás során csupán annyit teszel, hogy letiltod, hogy a te bejegyzésed alatt megjelenjen a troll / spam hozzászólás a többi között.

= Hogyan jeleníthetem meg a hozzászólások számát? =

Válaszd ki a sablonszerkesztés menüpontot és a sablonod bejegyzés (single.php) fájljába szúrd be a következő sort: `<?php if(function_exists('turulmeme_shares')){	turulmeme_shares('<h3>%d Google Reader hozzászólás</h3>'); } ?>`
A hozzászólások száma a %d helyére kerül.

== Screenshots ==

1. A bejegyzés alatt megjelenő lista
2. Admin rész

== Beállítások ==

A plugin meghívásakor lehetőségünk van módosítani, hogy mi jelenjen meg.

Csak a hozzászólások megjelenítése: `<?php if(function_exists('turulmeme_shares')){	turulmeme_shares('<h3>Google Reader hozzászólások</h3>'); } ?>`

Ha meg akarod jeleníteni, hogy kik osztották meg akár hozzászólás nélkül is a bejegyzést használd a plugin hívásnál a második paramétert valahogy így: `<?php if(function_exists('turulmeme_shares')){	turulmeme_shares('<h3>Google Reader hozzászólások</h3>', true); } ?>`

Az avatar képek méretének módosításához a plugin hívás harmadik paraméterével történik. Például ha 50*50-es avatarokat akarsz megjeleníteni akkor azt így tudod megtenni: `<?php if(function_exists('turulmeme_shares')){	turulmeme_shares('<h3>Google Reader hozzászólások</h3>', false, 50); } ?>`

