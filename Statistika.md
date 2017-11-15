---
permalink: Statistika
---

# TARA statistika

## Vajadus

Statistikavajadus tuleneb vajadusest:
- 1) tagada deklareeritud teenustase (SLA)
- 2) pidada väliste, tasuliste teenuste (DigiDocService) tarbimise arvestust
- 3) pidada arvestust teenuse kasutamise kohta klientide lõikes.

Statistika võib olla ka kasulik ka teenuse turvamisel.

Vajame statistilisi näitajaid (periood - kuu):
- kasutusstatistika
  - autentimiste arv
    - kokku
    - klientide lõikes (klient TARA mõistes on Eesti e-teenuse omanik-asutus)
      - klientrakenduste lõikes (kliendil võib olla mitu klientrakendust)
    - piiriülene/siseriiklik lõikes
      - välisriikide lõikes
    - autentimismeetodite lõikes
  - edukate autentimiste osakaal
- teenustaseme statistika
  - välisriigi teenuse maasoleku tõttu ebaõnnestunud autentimiste arv
  - välisriigi teenuste ülevaloleku protsent
  - Eesti TARA-välise teenuse maasoleku tõttu ebaõnnestunud autentimiste arv

Kõike võib-olla kohe teostada ei jõua, kuid järk-järgult. Piiriülene statistika muutub aktuaalseks siis, kui lisame eIDAS-autentimise.

Huvi pakuks ka palju siis erinevaid välismaalasi teenuses autenditakse? See nõuaks eIDAS-identifikaatorite andmebaasi pidamist. Keerukas ja oht, et problemaatiline andmekaitse seisukohalt. Kui, siis teises järjekorras.

Ülalesitatu ei sisalda SSO statistikat. SSO toob kaasa täiesti uued küsimused: Kui palju SSO-d kasutatakse? Mitmesse teenusesse SSO-ga sisse logitakse? Kes SSO-d kasutab?

## Tehniline lahendus

Alternatiivid:
- 1) majasisese ELK-stacki baasil
- 2) programmeerida eraldi statistikaotstarbeline logi + statistika arvutamise skript (majasisene)
- 3) välineteenus, in-premise paigaldus - Pivic
- 4) Google Analytics.

Statistika tootmiseks tuleks võimalusel kasutada oma lahendust. Google Analyticsile tuginemine, eriti kui teenust hakatakse laialdaselt kasutama, sh ühekordse sisselogimise režiimis, tekitab riski, et autentimisandmestik, kuigi sealt on isikukoodid ja nimed eemaldatud, võimaldab muude andmetega kombineerides teha järeldusi, mille võimalikku kasu või kahju me ei oska hinnata.

----

_Viimati muudetud: 15.11.2017_
