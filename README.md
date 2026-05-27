JS darbas tik su komandine eilute (prompt nukreipimas į terminalo langą).
Žingsniai atliekami jau sukūrus ir atsidarius projektą bei susikūrus pradinį .js failą.
Su node atkeliauja npm (node package manager), iš jo reikės papildomo modulio - prompt-sync. 
Po to prisidės viena eilutė .js failo pradžioje.

1. Inicializuojame npm (įgaliname paketų valdymą savo projekte). Terminalo lange vedama komanda:

npm init

Powershell gali mesti klaidą, VScode tada reikia atsidaryti terminalo langą Git Bash (+ dešinėje).
Gausime keletą užklausų įvesti informaciją (autorius, įvesties failas ir t.t.). Galima tiesiog suspaudinėti Enter.
Pabaigus projekte atsiras katalogas node_modules bei keletas failų.

2. Instaliuojame modulį prompt-sync. Komandinėje eilutėje:

npm install prompt-sync

3. .js failo pradžioje pridedame prompt nukreipimo kodą:

let prompt = require("prompt-sync")();

Failo pradžios pvz.:

"use strict";

let prompt = require("prompt-sync")();

//tolimesnis kodas

4. Džiaugamės, kad nebereikės muštis su alert'ais naršyklėje arba hardcode'inti.
Pastabos:

   alert() metodas nebeturės prasmės, rezultatus reikės spausdinti per console.log(); 
   pateikiant užduotį Teams reikia tik .js failų ir perspėti Mokytoją, kad atlikta su moduliu prompt-sync;
   kiekvienam naujam projektui reikės iš naujo instaliuoti prompt-sync (atlikti aukščiau esančius punktus). 
