# STATUS — Vellamo

Päivitetty: 2026-09-29

## Kesken nyt

✅ **29.9. sivusto päivitetty ja julkaistu** *(commit d2a744e, livenä varmistettu)*:
uusi `Hinnoittelu`-osio *(Lite, Pro, Enterprise hintahaarukoineen — alustava hinnasto,
Jaana 29.9.: hinnat saa käyttää)*, Vuorojen suunnittelu merkitty Pro- ja
Enterprise-tasoille, Raportointi- ja Uimataidon seuranta -tekstit kertovat mitä tiedolla
voi tehdä. `llms.txt` päivitetty samalla; JSON-LD ei sisällä hintoja.
todenna: `curl -s https://www.hailervellamo.com/ | grep -c 'id="hinnoittelu"'`

Kaksi siivousasiaa on kirjattu
**ylläpitovelkaan** *(`~/Hailer/KONTEKSTIVELKA.md`)*, koska ne eivät ole sisältötyötä:
⚠️ **niiden korjaus vaatii luvan rivi kerrallaan** eikä tapahdu muun työn sivutuotteena.

- `vellamo_website.html` poistetaan ja osoite ohjataan. Tiedosto on tunnettu 25.5. jäänne
  *(dokumentoitu kymmenessä `PROMPT_*.md`-tiedostossa)* ja poistopäätös tehtiin jo 12.8.
  Uutta 30.8.: se vastaa julkisesti 200:lla, eli on kaksoiskappalesisältöä.
- `.gitignore` puuttuu, `.DS_Store` on pushattu. Ei vuoda mitään.

Viimeisin commit (18e7986) lisäsi Google Search Console -vahvistustunnisteen; sitä
ennen poistettiin Google Analytics ja lisättiin Hailerin vakiokuvaus alatunnisteeseen,
llms.txt:hen ja JSON-LD-rakennedataan.

## Seuraava askel

**Lisää Vantaan asiakastarina sivustolle** (oma osio tai linkki `Hinnoittelu`- ja
`Käyttöönotto`-osioiden väliin) **kun tarina on hyväksytty ja julkaistu.** Hyväksyntä
odottaa Milaa — ks. `hailer-gtm/asiakastarinat/vantaa-vellamo/STATUS.md`.

## Odottaa

- **Pia vahvistaa Timo Ahoselta: kuuluvatko oppilaskohtaiset PDF-tulosteet Lite-tasolle**
  *(Jaana antoi kysymyksen Pialle 29.9.; Timon välitetty vastaus Pialta 29.9.: «voi olla jo
  ekassa mukana»)*. Sivustolla PDF-lause
  on nyt tasoa mainitsematta `Uimataidon seuranta` -kortissa — jos PDF onkin vain Prossa,
  sivu pitää korjata.
  todenna: ihmislähde, kysy Pialta
- **Pia vahvistaa Timo Ahoselta: onko huoltajille lähettäminen automaattista Pro-tasolla jo nyt vai
  suunnitteilla** *(Jaana antoi kysymyksen Pialle 29.9.)*. Pia kuvaa lähettämisen nykyisin
  manuaaliseksi.
  todenna: ihmislähde, kysy Pialta

## Päätökset joita ei saa perua

- **2026-09-29 (Jaana):** hinnat saa näyttää sivustolla. Osion nimi on «Hinnoittelu»,
  ei «Laajuudet». Hinnasto on alustava; hinnoittelun vahvistus ei ole viestinnän päätös.
- Google Analytics poistettu, Vercel Insights jää (commit bad3e98).

## Viitteet

- GitHub: `HailerOy/vellamo`
- `hailer-gtm/KUVAUS_HAILER.md` — vakiokuvaus jota alatunniste käyttää
