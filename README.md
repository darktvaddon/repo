# IPTV Balkan — Kodi dodatak

> ### ⬇️ Za instalaciju preuzmite samo ovu datoteku:
> ### **[repository.iptvbalkan-1.0.0.zip](https://raw.githubusercontent.com/darktvaddon/repo/main/repository.iptvbalkan-1.0.0.zip)**
>
> Nemojte koristiti zeleno dugme **„Code → Download ZIP"**. Ono preuzima ceo repozitorijum
> (`repo-main.zip`), koji Kodi odbija — to nije dodatak, nego kopija ovog spiska datoteka.

IPTV Balkan reprodukuje **vašu sopstvenu pretplatu**. Prijavljuje se na nalog koji već plaćate, od
njega gradi listu kanala i televizijski vodič, a reprodukciju prepušta Kodijevim ugrađenim plejerima.
Dodatak ne sadrži sopstvene tokove niti tuđi sadržaj — sve što se pojavi na ekranu dolazi sa vašeg
naloga.

## Mogućnosti

* **Televizija i vodič** — kanali se pojavljuju u Kodijevoj TV sekciji, sa grupama, logotipima i
  programskim vodičem, kao da ih pruža sam Kodi. Radio stanice dobijaju svoju sekciju.
* **Arhiva** — emisija od juče ili od pre nedelju dana pokreće se direktno iz vodiča, kod operatera
  koji tu uslugu nude.
* **Video klub** — filmovi i serije sa vašeg naloga, sa opisima, plakatima i ocenama.
* **Nastavak reprodukcije** — prekinut film nastavlja se tačno odatle, na svim izvorima.
* **Pretraga** — kroz kanale, vodič i Video klub istovremeno.
* **Više naloga** — dve pretplate kod istog operatera rade uporedo.
* **Unos naloga telefonom** — lozinka se ne kuca daljinskim upravljačem: televizor prikaže QR kod, a
  podaci se popunjavaju na telefonu.

### Podržani izvori

| Izvor | Kanali | Vodič | Arhiva | Video klub |
|---|:--:|:--:|:--:|:--:|
| **EON** | ✔ | ✔ | ✔ | ✔ |
| **Iris (MTS)** | ✔ | ✔ | ✔ | ✔ |
| **Yettel** | ✔ | ✔ | ✔ | ✔ |
| **Move (MTS)** | ✔ | ✔ | — | — |
| **Xtream panel** | ✔ | ✔ | ako je panel pruža | ✔ |
| **M3U / XMLTV lista** | ✔ | uz XMLTV adresu | ako je lista sadrži | filmovi iz liste |

---

## Instalacija

1. Preuzmite **[repository.iptvbalkan-1.0.0.zip](https://raw.githubusercontent.com/darktvaddon/repo/main/repository.iptvbalkan-1.0.0.zip)** (veza iznad).
2. U Kodiju otvorite **Dodaci → ikonica za pregled dodataka (gore levo) → Instaliraj iz zip
   datoteke** i izaberite preuzetu datoteku.
3. Zatim **Dodaci → Instaliraj iz repozitorijuma → IPTV Balkan repozitorijum → Video dodaci →
   IPTV Balkan → Instaliraj**.

To je sve. Potrebne komponente (`pvr.iptvsimple`, `inputstream.adaptive`, `inputstream.ffmpegdirect`)
Kodi instalira samostalno, a nova izdanja od tog trenutka stižu kroz njegovu redovnu proveru — zip
datoteka više nije potrebna.

Ako Kodi odbije da instalira zip datoteku, uključite:
**Podešavanja → Sistem → Dodaci → Nepoznati izvori.**

## Unos naloga

**Dodaci → IPTV Balkan → Nalozi i uređaji → Unesi nalog sa drugog telefona (QR).**

Televizor prikazuje QR kod. Skenirajte ga telefonom povezanim na istu Wi-Fi mrežu, popunite obrazac i
potvrdite — podaci naloga stižu na televizor bez kucanja daljinskim upravljačem. Odmah zatim dodatak
nudi preuzimanje liste kanala i vodiča; prvo preuzimanje traje nekoliko minuta jer se povlači ceo
vodič, a nakon toga se osvežava jednom dnevno, u pozadini.

Isti podaci mogu se uneti i ručno, u **Podešavanjima** dodatka.

## Nova izdanja

Kodi proverava repozitorijume **na svakih šest sati**, i to je jedini raspored — nova verzija zato ume
da se pojavi i nekoliko sati nakon objavljivanja. To nije kvar ni repozitorijuma ni dodatka.

**Ako vam je potrebna odmah:** otvorite **Dodaci → Instaliraj iz repozitorijuma → IPTV Balkan
repozitorijum → Video dodaci**. Samo otvaranje tog spiska primorava Kodi da preuzme svež indeks, pa se
nova verzija odmah prikazuje, sa dugmetom *Ažuriraj*. Isključivanje i uključivanje repozitorijuma,
kao ni dugme za osvežavanje, ne postižu to pouzdano.

> **Ako ste dodatak ranije instalirali iz zip datoteke, Kodi ga neće ažurirati.** Kodi ažurira samo
> ono čijeg se izvora seća, a zip datoteka izvor nema. Ponovite korak 3 iz instalacije; Kodi će
> najaviti da će prethodna verzija biti *deinstalirana i zamenjena*, što je očekivano — nalozi,
> podešavanja i zapamćene pozicije reprodukcije ostaju netaknuti. Nakon toga ažuriranja stižu
> automatski.

## Rešavanje problema

* **Nema kanala nakon instalacije** — nalog najverovatnije nije unet, ili prvo preuzimanje još traje.
  Otvorite **Osveži kanale i vodič sada**; taj ekran prikazuje šta je svaki izvor odgovorio.
* **Jedan izvor ne radi, ostali rade** — očekivano stanje koje dodatak podnosi: ostali izvori dobijaju
  svež vodič, a izvor koji se nije javio zadržava poslednji sačuvani spisak dok ponovo ne bude
  dostupan.
* **Ništa se ne pokreće, bez jasnog razloga** — **Pomoć, licenca i dijagnostika → Pošalji poruku
  podršci (sa logom)** šalje opis problema i dijagnostiku odjednom. Dnevnik rada može se pregledati i
  na licu mesta ili preuzeti telefonom preko QR koda, iz istog menija.
* **Pitanja i prijave** — [Telegram grupa](https://t.me/+d7XjefqrYkkyYjlk).

## Zahtevi

Kodi 20 ili noviji, na bilo kojoj platformi (Android, Windows, Linux, LibreELEC, macOS). Dodatak je
napisan u Pythonu i jedna ista zip datoteka radi svuda — nema posebnih izdanja po uređaju.

## Sadržaj repozitorijuma

Ovde se nalaze isključivo datoteke potrebne za instalaciju; izvornog koda nema.

| Datoteka | Namena |
|---|---|
| `repository.iptvbalkan-1.0.0.zip` | **instalira se prilikom prvog postavljanja** |
| `addons.xml`, `addons.xml.md5` | indeks koji Kodi čita |
| `plugin.video.iptvbalkan/` | izdanja dodatka, koja Kodi preuzima samostalno |

Podaci o filmovima i serijama dolaze sa [TMDB-a](https://www.themoviedb.org/); ovaj dodatak TMDB nije
odobrio niti sertifikovao. Ikone u meniju su Material Symbols (Google, Apache-2.0).

---

## English

> ### ⬇️ Download this file only:
> ### **[repository.iptvbalkan-1.0.0.zip](https://raw.githubusercontent.com/darktvaddon/repo/main/repository.iptvbalkan-1.0.0.zip)**
>
> Do not use the green **“Code → Download ZIP”** button. It gives you a copy of this file listing
> (`repo-main.zip`), which Kodi will refuse — it is not an add-on.

IPTV Balkan plays **your own subscription**. It signs in to the account you already pay for, builds a
channel list and an electronic programme guide from it, and hands playback to Kodi's own players. The
add-on carries no streams and no third-party content of its own.

**Features.** Channels and EPG in Kodi's native TV section, with groups and logos; catch-up straight
from the guide where the operator offers it; an on-demand library with descriptions, posters and
ratings; resume where you left off; search across channels, guide and library at once; several
accounts with the same operator side by side; and account entry from a phone via an on-screen QR code,
so no password is typed with a remote control.

**Supported sources.** EON, Iris (MTS), Yettel, Move (MTS), any Xtream panel, and plain M3U/XMLTV
playlists — with catch-up and an on-demand library wherever the source provides them.

**Installation.** Kodi → Add-ons → *Install from zip file* → the file above → then *Install from
repository* → IPTV Balkan → Video add-ons → IPTV Balkan. Kodi installs the required components
(`pvr.iptvsimple`, `inputstream.adaptive`, `inputstream.ffmpegdirect`) by itself, and every later
release arrives through its normal update check, which runs every six hours. If Kodi refuses the zip
file, enable **Settings → System → Add-ons → Unknown sources**.

**Requirements.** Kodi 20 or newer, on any platform (Android, Windows, Linux, LibreELEC, macOS). The
add-on is written in Python and a single zip file works everywhere.

**Support.** [Telegram group](https://t.me/+d7XjefqrYkkyYjlk).

Film and series metadata is provided by [TMDB](https://www.themoviedb.org/). This product uses the
TMDB API but is not endorsed or certified by TMDB. Menu icons are Material Symbols (Google,
Apache-2.0).
