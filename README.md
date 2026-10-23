# nn-dnevno

Dnevni pregled novih propisa objavljenih u službenom dijelu
[Narodnih novina](https://narodne-novine.nn.hr/), od 1. siječnja 2026.

Ovdje se nalaze:

- **`editions.json`**: popis brojeva NN, najnoviji prvi. Za svaki broj tu su datum objave i
  `added_at` (kada je stigao ovamo), a za svaki propis naslov, vrsta, ELI poveznica i putanja
  do datoteke.
- **`zakoni/{godina}/NN-{broj}-{redni broj}.md`**: tekst svakog propisa u Markdownu, s
  metapodacima (naslov, ELI, vrsta, datumi, donositelj) u YAML zaglavlju.

Svako ažuriranje s novim propisima je jedan commit, s naslovima propisa u poruci.

## Kako provjeriti ima li nešto novo

- Popis: <https://raw.githubusercontent.com/ivananic779/nn-dnevno/main/editions.json>.
  Najnoviji brojevi su na vrhu.
- Commitovi kao Atom feed: <https://github.com/ivananic779/nn-dnevno/commits/main.atom>
- Tekst propisa: `https://raw.githubusercontent.com/ivananic779/nn-dnevno/main/` + vrijednost
  `file` iz `editions.json`, npr.
  <https://raw.githubusercontent.com/ivananic779/nn-dnevno/main/zakoni/2026/NN-120-1427.md>

Ažurira se radnim danom, obično između 13 i 17 h UTC. Broj objavljen subotom pojavljuje se u
ponedjeljak.

## Ovo nisu službeni tekstovi

Datoteke su strojna pretvorba HTML stranica Narodnih novina, a pretvorba nije savršena:
tablice su pojednostavljene, a akti objavljeni samo kao PDF ovdje nedostaju.
**Službeni tekst propisa je onaj objavljen u Narodnim novinama.** Ništa ovdje nema pravnu
snagu i ne treba se na to oslanjati bez provjere u Narodnim novinama.
