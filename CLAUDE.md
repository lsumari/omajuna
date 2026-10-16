# omajuna

omajuna on yhden tiedoston junalähtönäyttö. Projektissa on vain kaksi tiedostoa:

- `index.html`: koko sovellus, CSS ja JavaScript samassa tiedostossa
- `icon.png`: kuvake

## Rajoitteet

- Ei kirjastoja, frameworkeja eikä build-työkaluja. Älä lisää riippuvuuksia, `package.json`-tiedostoa tai erillisiä CSS- tai JS-tiedostoja.
- Julkaistaan GitHub Pagesissa julkisesta repositoriosta. Ei salaisuuksia eikä henkilötietoja repositorioon.
- Data haetaan selaimesta Digitrafficin rajapinnasta (rata.digitraffic.fi). API-avainta ei ole eikä sellaista lisätä.

## Käyttöliittymä

- Käyttöliittymän teksti on suomea.
- Ajat näytetään Europe/Helsinki-aikavyöhykkeellä, riippumatta laitteen aikavyöhykkeestä.

## Asetukset

- Asetukset annetaan URL:ssä, esim. `?asema=LPV&kohde=HKI&linjat=A,E`.
- Pidä URL-parametrit toimivina: älä nimeä niitä uudelleen tai muuta niiden merkitystä rikkomatta olemassa olevia linkkejä.

## Testaus

Avaa `index.html` selaimessa osoitteella `?asema=LPV&kohde=HKI`.

Älä avaa sisäistä selainpaneelia (Browser pane) äläkä käytä `mcp__Claude_Browser__*`-työkaluja tämän projektin testaamiseen. Paneeli avaa `index.html`:n `data:`-osoitteena, jolloin URL-parametrit katoavat, eikä ohjetekstin linkkikään toimi (`about:blank#blocked`). Älä yritä kiertää tätä paikallisella palvelimella. Käyttäjä testaa itse oikeassa selaimessa Claude Desktopin ulkopuolella. Kerro muutoksen jälkeen, mitä pitää tarkistaa, äläkä yritä varmistaa ulkoasua itse selaimella.

Kun sivu avataan ilman parametreja, se näyttää ohjetekstin, jossa on klikattava esimerkkilinkki (`?asema=LPV&kohde=HKI`). Pidä linkki ohjetekstissä.

## Git

Älä tee committeja äläkä pushaa. Käyttäjä hoitaa ne itse.
