# Ajastin – Aika- ja hälytyssovellus

Suomenkielinen ajastinsovellus, joka on suunniteltu erityisesti helppokäyttöisyyteen ja näkyvyyteen kauempaakin. Sovellus toimii selaimessa ja sitä voi käyttää myös PWA-sovelluksena puhelimessa tai tietokoneella.

🔗 **Live-versio**: [https://samuelkallio.github.io/Ajastin/](https://samuelkallio.github.io/Ajastin/)

---

## 📋 Ominaisuudet

- ✅ **Ajastimen asetus** minuutteina ja sekunteina (max 999 min)
- ✅ **Käynnistä, Tauko, Jatka ja Keskeytä** – keskeytys vaatii vahvistuksen
- ✅ **Minimalistinen täysnäyttötila** ajastimen käydessä – kello suurena ja vain oleelliset toiminnot näkyvissä
- ✅ **Näytön hereilläpito (Wake Lock)** – näyttö pysyy päällä koko ajan (selaimen tuki huomioiden)
- ✅ **Summeriäänen valinta** kolmesta vaihtoehdosta (horn, ice hockey, school bell) ja esikuuntelu
- ✅ **Sovelluksen jakaminen** linkillä tai QR-koodilla
- ✅ **Sisäänrakennettu käyttöohje** ja versionumero, josta voi tarkistaa päivitykset
- ✅ **PWA-valmius** – asennettavissa puhelimen aloitusnäytölle
- ✅ **Sulje sovellus** -painike PWA-tilaa varten

---

## 🚀 Käyttöohje

1. **Aseta aika**: Syötä minuutit ja sekunnit kenttiin.
2. **Käynnistä**: Paina **Käynnistä**-painiketta.
3. **Ajastimen käydessä**: Näet vain suuren kellon ja **Tauko**-painikkeen.
4. **Tauko**: Paina **Tauko** – tilaan tulevat **Jatka** ja **Keskeytä**.
   - **Keskeytä** avaa varmistusdialogin; vahvistus nollaa ajastimen.
5. **Hälytys**: Kun aika loppuu, summeri soi 3 sekuntia ja kello vilkkuu. Paina **Nollaa** lopettaaksesi hälytyksen.
6. **Summeriäänen vaihto**: Paina **Summeri**-painiketta ja valitse haluamasi ääni radio-painikkeella. Kuuntele esimakua ▶-kuvakkeesta.
7. **Ohje ja versio**: Paina **?**-painiketta lukeaksesi ohjeet. Versionumerosta (esim. 1.2.0) voit tarkistaa päivitykset.
8. **Sovelluksen jakaminen**: Paina **🔗**-painiketta kopioidaksesi linkin tai näyttääksesi QR-koodin.
9. **Sulje sovellus**: Paina **✕**-painiketta (toimii PWA-tilassa).

---

## 🛠️ Teknologiat

- **HTML5**, **CSS3**, **Vanilla JavaScript**
- **Wake Lock API** – näytön hereilläpito
- **Web Audio API** – varasummeri (fallback)
- **PWA** – asennettavuus ja offline-tuki (manifest ja service worker mahdollistettu)
- **QR-koodi** – dynaaminen generointi `api.qrserver.com` -palvelun kautta

---

## 📦 Asennus ja käyttöönotto

Sovellus on yksittäinen HTML-tiedosto, joka toimii sellaisenaan. Voit käyttää sitä suoraan verkkosivuna tai asentaa sen PWA:na.

### Paikallinen ajo
1. Lataa `index.html`-tiedosto.
2. Avaa tiedosto selaimessa.

### Julkaisu GitHub Pagesiin
1. Forkkaa tai kopioi tämä repositorio.
2. Ota GitHub Pages käyttöön repositorion asetuksista.
3. Sovellus on käytettävissä osoitteessa `https://<käyttäjätunnus>.github.io/<reponimi>/`.

### PWA-asennus
- **Android (Chrome)**: Avaa sovellus selaimessa → valitse "Lisää aloitusnäyttöön".
- **iOS (Safari)**: Avaa sovellus → jaa → "Lisää aloitusnäyttöön".
- **Tietokone (Edge/Chrome)**: Avaa sovellus → osoiteriviltä → "Asenna sovellus".

---

## 🔄 Päivittäminen

Sovellus tarkistaa versionumeroa. Kun painat versionumeroa (esim. `1.2.0`) ohjemodaalissa, sovellus kysyy haluatko päivittää uusimpaan versioon. Päivitys lataa sivun uudelleen palvelimelta (välimuisti ohitetaan).

Jos haluat päivittää manuaalisesti, voit tyhjentää selaimen välimuistin tai ladata sivun uudelleen `Ctrl+F5` (tai `Cmd+Shift+R`).

---

## 📄 Lisenssi

Tämä projekti on julkaistu [MIT-lisenssillä](LICENSE). Voit vapaasti käyttää, muokata ja jakaa sitä.

---

## 📝 Versiohistoria

- **1.2.0** – Päivitetty käyttöliittymä: ohje-, jako- ja sulkemispainikkeet, versiolinkki, wake lock aina päällä
- **1.1.0** – Summeriäänivalinta, esikuuntelu, modaalit
- **1.0.0** – Ensimmäinen julkaisu: perusajastin, tauko, keskeytys, hälytys

---

## 🤝 Osallistuminen

Parannusehdotukset ja ongelmaraportit ovat tervetulleita. Voit tehdä pull requestin tai avata issuen.

---

**Kiitos käytöstä!** 🕒