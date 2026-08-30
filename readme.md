# Vefforritun 1, 2026: Verkefni 1, HTML

Útgáfa 0.4.

## Markmið

- Setja upp textaritil og búa til möppur og skrár.
- Vinna með og velja HTML element.
- Nota HTML validator og huga að því hvernig HTML er skrifað.
- Nota Netlify til að gera verkefni aðgengilegt á internetinu.
- Huga að aðgengi og nota aXe tólið.

## Verkefni 2–6

Í verkefnum 1, 2 og 3 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 1](https://github.com/vefforritun/vef1-2026-v1) skilgreinir HTML og síður.
- [Verkefni 2](https://github.com/vefforritun/vef1-2026-v2) setur upp útlit með CSS.
- [Verkefni 3](https://github.com/vefforritun/vef1-2026-v3) gerir útlit skalanlegt (e. responsive) með CSS og setur upp tól til að hjálpa við vinnu og skipulag.

## Lýsing

Setja skal upp fjórar síður fyrir ferðaþjónustufyrirtæki, aðgengilegar af internetinu (gegnum Netlify):

- Forsíða ferðaþjónustufyrirtækis.
- Um ferðaþjónustufyrirtækið.
- Yfirlit yfir ferðir.
- Skráning í ferð.

## Efni og möppur

Gefið efni er í textaskrám undir [`gogn/`](gogn/) og er á Markdown formi. Ekki á að birta nákvæmlega það efni sem kemur fram heldur fylgja leiðbeiningum í hverri skrá fyrir sig og því sem kemur fram hér.

Athugið að ef Markdown skjal er opnað á GitHub er það birt sem HTML og sýnir útlit sem ekki skal nýta, t.d. eru línur undir fyrirsögnum. Til að sjá eingöngu Markdown skjalið er „raw“ útgáfa valin í vefviðmóti GitHub eða allt [verkefnið sótt sem zip skjal](https://github.com/vefforritun/vef1-2026-v1/archive/refs/heads/main.zip). Að sækja sem zip skjal er betri leið þar sem þá er einnig hægt að vinna verkefnið út frá þeirri möppu.

Gefnar myndir eru í `myndir/` og skal vísa í þær þar. Nota þarf „relative“ vísun úr `sidur/` yfir í `myndir/` þar sem við á. Myndir skulu ekki færðar. Leyfilegt er að minnka myndir eða setja `width` eigindi (attribute) á mynd (`<img>` element) til að takmarka breidd þeirra.

Gefin er tóm mappa `sidur/` sem skal innihalda allar síður _fyrir utan_ forsíðuna, hún er í rótinni sem `index.html`.

Myndir:

- [Mynd af fossi](myndir/seljalandsfoss.jpg)
  - Lýsing á mynd: Mynd af Seljalandsfossi, tekin úr brekku og horft yfir landslagið. Fossinn er hægra megin og vinstra megin má sjá grænt gras og nokkrar manneskjur.
  - [Frá Unsplash](https://unsplash.com/photos/waterfalls-at-daytime-zNN6ubHmruI?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) eftir [Robert Lukeman](https://unsplash.com/@robertlukeman?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
- [Mynd af vegi](myndir/vegur.jpg)
  - Lýsing á mynd: Mynd af malbikuðumvegi á Íslandi. Vegurinn er fyrir miðju og fer áfram út að sjóndeildarhringnum, vinstra megin er fjall, hægra megin er himinn.
  - [Frá Unsplash](https://unsplash.com/photos/asphalt-road-and-cliff-horizon-PBrovES5uuI?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) eftir [Rory Hennessey](https://unsplash.com/@roryhennessey?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

## Síður

### Sameiginlegt

Allar síður skulu:

- Nota `utf-8` stafasett.
- Allar síður skulu byggja á minnsta HTML skjalinu samkvæmt námsefni.
- Allar síður skulu hafa titil með viðeigandi HTML element.
- Innihalda valmynd sem vísar á allar aðrar síður og merkja valda síðu á einhvern hátt, heiti tengla skulu vera:
  - Forsíða
  - Um fyrirtækið
  - Ferðir
  - Skráning í ferð
- Hafa fót (gögn neðst á síðunni) með upplýsingum um opnunartíma, staðsetningu og samfélagsmiðla (notum HÍ samfélagsmiðla sem hlekki), sjá [`gogn/fotur.md`](gogn/fotur.md).
- Hafa lýsigögn skilgreind fyrir `description`, `og:title`, `og:description` og `og:image` (veljið aðra hvora mynd úr `/myndir`). Prófið með [OpenGraph Social Previewer](https://www.opengraph.xyz/) til að sjá hvort gögn séu rétt eftir að síða er sett upp á Netlify.
- Hafa tengil neðst í efni með textanum „Aftur á forsíðu“. Á ekki við forsíðu.
- Hafa fyrisögn og „beint í efni“ hlekk á eftir fyrirsögn, en á undan valmynd. Hlekkur sem leyfir þeim sem nota skjálesara að sleppa við að hlusta á valmynd.

### Forsíða

`index.html`, forsíða með texta tilgreindum í [`gogn/index.md`](gogn/index.md).

Inniheldur inngangstexta og yfirlit með smá texta, mynd og vísun á síðu.

### Um síða

Síðan skal eiga heima undir `sidur/um.html`, með texta og myndum í [`gogn/um.md`](gogn/um.md).

### Yfirlit yfir ferðir

Birta fyrirsögnina „Ferðir“ og síðan lista yfir ferðir sem eru í boði.

Listi af ferðum er í [`gogn/ferdir.csv`](gogn/ferdir.csv). Fyrir hverja ferð eru eftirfarandi upplýsingar skráðar og skal birta:

- Heiti ferðar
- Stutt lýsing á ferð
- Lengd ferðar í klukkustundum
- Erfiðleikastig ferðar, eitt af „Auðveld“, „Miðlungs“ eða „Erfið“
- Tímabil sem ferð er í boði, eitt af eftirfarandi: „Allt árið“, „Sumar“ eða „Vetur“
- Verð ferðar per manneskju í íslenskum krónum

Það má nota hvaða leið sem þið viljið til að koma gögnum úr CSV formi ([„Comma-separated values“](https://en.wikipedia.org/wiki/Comma-separated_values)) yfir í HTML, t.d. með því að gera alveg í handvirkt, nota virkni í ritli eða forrita.

### Skráningarsíða

Síða með formi til að skrá sig í ferð, formið skiptist í fjögur svæði sem hafa mismunandi reiti með lýsingu, reit til að skrá eða velja upplýsingar úr og hugsanlega auka upplýsingum sem ber að túlka þegar viðeigandi HTML element er valið/valin:

- Ferð
  - „Hvaða ferð viljið þið skrá ykkur á?“
    - Val um allar ferðir sem eru í boði.
- Hópur
  - „Fjöldi í hóp“
    - Val um fjölda í hóp, heiltala frá einum. Megið ráða hámarki.
    - Krafa að velja, verður að vera heiltala.
  - „Upplýsingar um hóp“
    - Textareitur fyrir upplýsingar um hóp
    - Auka texti sem fylgir: „Hver er reynsla hópsins?“
    - Krafa að skrifa í.
  - „Netfang tengiliðar“
    - Texti sem lítur út fyrir að vera netfang
    - Verður að fylla út í.
  - „Símanúmer“
    - Texti sem lítur út fyrir að vera símanúmer (000-0000)
    - Þarf ekki að fylla út í.
- Dagsetning og tími
  - „Hvenær viljið þið koma?“
    - Val um dagsetningu, þarf ekki að vera takmörkuð, bundin við ákveðna daga eða tengd valinni ferð. Einföld uppsetning.
    - „Hvaða tíma?“
      - Val um „Fyrir hádegi“, „Eftir hádegi“ og „Kvöld“.
      - Ekki þarf að takmarka við gefin opnunartíma út frá degi sem valinn er
      - Krafa að velja gildi.
- Bóka
  - „Samþykki skilmála“
    - Box sem hægt er að haka í.
    - Texti skal vera hlekkur sem fer á skilmála síðu, en þar sem hún er ekki til skal nota „Um“ síðu. Síðan skal opnast í nýjum glugga/tab.
  - „Panta og greiða“, takki sem sendir pöntun (en gerir ekki neitt)

Aðeins á að setja upp formið, **engin** forritun fyrir virkni í formi með JavaScript eða í bakenda. Þegar formið er sent á ekkert að gerast, jafnvel þó síðan hlaðist inn aftur og engin gögn séu til staðar er það í fínu lagi.

### Lýsigögn fyrir síður

- Forsíða
  - Titill: „Ferðaþjónustufyrirtækið“
  - Lýsing: „Við bjóðum upp á fjölbreytt úrval af ferðum allan ársins hring.“
- Um síða
  - Titill: „Um Ferðaþjónustufyrirtækið“
  - Lýsing: „Lærðu meira um okkur og okkar starfsemi.“
- Ferðasíða
  - Titill: „Ferðir“
  - Lýsing: „Skoðaðu ferðirnar okkar.“
- Skráningarsíða
  - Titill: „Skráning í ferð“
  - Lýsing: „Skráðu þig í þína draumaferð.“

## Merkingarfræðileg element og validators

- **Nýta skal merkingarfræðilega viðeigandi element**.
- Passa skal upp á að hafa snyrtilega uppsettan kóða þar sem inndráttur er samræmdur.
- Allar síður skulu vera villulausar ef prófaðar með [HTML validator](https://validator.w3.org/).
- Allar síður skulu vera án aðgengisvillna ef prófaðar með [aXe](https://www.deque.com/axe/), setjið upp viðbót í vafra.

Ef [prettier](https://prettier.io/) er notað innan vscode þá mun HTML validator koma með upplýsingar (`Info`) um að „Trailing slash on void elements has no effect and interacts badly with unquoted attribute values.“, þetta er í lagi.

## Netlify

Setja skal upp verkefni á Netlify með því að hlaða upp skrám með „manual deploy“ _eða_ tengja GitHub repo. Einnig er leyfilegt að nota aðra hýsingu en heyrið í kennara varðandi það.

## Útlit

Ekki er gefin forskrift að útliti, þar sem verkefnið snýst um að setja upp merkingarfræðilegt HTML sem snýst um að huga að merkingarfræði _ekki_ útliti.

Ekki skal útfæra neitt CSS. Ef ekki er farið eftir því og CSS er útfært verður það að falla að framtíðarkröfum námskeiðs og vera uppsett samkvæmt þeim, ef svo er ekki verður einkunn lækkuð.

## Mat

- 15% – Sameiginlegt efni uppsett eftir forskrift.
- 10% – Forsíða uppsett eftir forskrift.
- 10% – Um síða uppsett eftir forskrift.
- 15% – Ferðayfirlitssíða uppsett eftir forskrift.
- 20% – Skráningarsíða uppsett eftir forskrift.
- 25% – Merkingarfræðileg element og síður án villna frá HTML validator og aXe validator.
- 5% – Verkefni aðgengilegt á vef gegnum Netlify og rétt sett upp þar.

## Sett fyrir

Verkefni sett fyrir í fyrirlestri mánudaginn 17. ágúst 2026.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 3. september 2026.

Skilaboð skulu innihalda bæði:

- zip skrá með öllum skrám og möppum í lausn á verkefni (eða hlekkur á GitHub).
- slóð á verkefni keyrandi á Netlify, sett sem athugasemd við skil á Canvas.

Athugið að það er **ekki nóg** að eingöngu setja athugasemd, skila þarf verkefni sérstaklega. Verkefnum sem ekki er skilað fá ekki einkunn.

## Aðstoð

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ekki er heimilt að nota stór mállíkön til að vinna verkefni í námskeiðinu, [sjá nánar um notkun](https://github.com/vefforritun/vef1-2026/blob/main/mallikon.md).

## Verkefni og einkunn

Sett verða fyrir fimm minni verkefni sem gilda 3% hvert, samtals 15% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 5%, samtals 10% af lokaeinkunn.

---

Nýjustu útgáfu af verkefni má [nálgast á GitHub](https://github.com/vefforritun/vef1-2026-v1).

## Útgáfusaga

| Útgáfa | Lýsing                                                                      |
| ------ | --------------------------------------------------------------------------- |
| 0.1    | Fyrsta útgáfa                                                               |
| 0.2    | Bæta við lýsigögnum fyrir allar síður; laga innsláttarvillur í `ferdir.csv` |
| 0.3    | Uppfæra lýsigagnaleiðbeiningar; uppfærsla eftir fyrirlestur 2               |
| 0.4    | Réttar upplýsingar um einkunn verkefna                                      |
