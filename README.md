# Vefforritun 1, 2023: Verkefni 6, CSS #4

## Markmið

- Setja upp Node.js og NPM og nota til að sækja pakka.
- Nota tól fengin af NPM.
- Keyra tól í vinnuflæði með `package.json`.

Vinna má út frá [sýnilausn á verkefni 5](https://github.com/vefforritun/vef1-2023-v5-synilausn).

## Verkefni 2–6

Í verkefnum 2–6 munum við vinna áfram með sama verkefni og byggja ofan á það:

- [Verkefni 2](https://github.com/vefforritun/vef1-2023-v2) skilgreinir grunn HTML og síður.
- [Verkefni 3](https://github.com/vefforritun/vef1-2023-v3) bætir við grunn viðmóti.
- [Verkefni 4](https://github.com/vefforritun/vef1-2023-v4) setur upp útlit (e. layout).
- [Verkefni 5](https://github.com/vefforritun/vef1-2023-v5) setur upp grind og gerir útlit skalanlegt (e. responsive).
- [Verkefni 6](https://github.com/vefforritun/vef1-2023-v6) setur upp tól til að hjálpa við skipulag og vinnu.

## Útlit

Sama gildir um útlit og í verkefni 5, útlit ætti að haldast alveg það sama, eina sem breytist er hvernig verkefnið er uppsett.

## Tæki og tól

Til þess að geta notað þessi tól þarf að [setja upp Node.js, sækið „Recommended For Most Users“](https://nodejs.org/en/). Eftir að þið hafið keyrt uppsetningar forrit getið þið opnað Command prompt/terminal/skel og keyrt:

```bash
> node -v
v18.18.1 # eða sú útgáfa sem þið sóttuð
> npm -v
9.8.1 # eða álíka
```

Ef þið fáið þetta ekki upp, prófið að endurræsa. Annars fá aðstoð í dæmatímum, í fyrirlestri, tölvupósti eða á slack.

Setja skal upp `sass`, `browser-sync`, `stylelint` og `concurrently` til að nýta Sass og geta gert breytingar sem sjást strax í vafra.

Fyrst þarf að búa til `package.json` með því að keyra `npm init` í verkefnamöppu.

Síðan þarf að sækja hvert tól með `npm install <nafn á tóli>`.

### Sass

Skipta skal CSS upp í mismunandi skrár undir `styles/`.

Í `styles/config.scss` skal geyma allar stillingar fyrir verkefni og nota þær á viðeigandi stöðum.

### Browser sync & concurrently

Þegar skipunin `npm run dev` er keyrð skal verkefnið keyra upp vefþjón með `browser-sync`, þýða sass skrár og fylgjast með breytingum á HTML og Sass.

### Linting

Setja skal upp stylelint með `stylelint-config-sass-guidelines`, `.stylelintrc` ætti að innihalda:

```
{
  "extends": ["stylelint-config-sass-guidelines"],
  "rules": {}
}
```

Þegar skipunin `npm run lint -s` er keyrð skal keyra stylelint með þessum reglum og ættu engar villur að koma fram.

## Mat

- 30% – CSS flutt yfir í Sass
- 30% – stylelint uppsett og engar villur
- 20% – Verkefni sett upp með git, repo á GitHub og tengt þaðan við Netlify
- 20% – Verkefni sett upp með `package.json` og viðeigandi scriptum

## Sett fyrir

Verkefni sett fyrir fyrst á Canvas mánudaginn 2. október 2023 og af alvöru í fyrirlestri mánudaginn 9. októkber 2023.

## Skil

Skila skal í Canvas, seinasta lagi fyrir lok dags fimmtudaginn 19. október 2023.

Skilaboð skulu innihalda:

- Slóð á verkefnið keyrandi í hýsingu
- Slóð á GitHub repo fyrir verkefni. Dæmatímakennurum skal hafa verið boðið í repo. Notendanöfn þeirra eru:
  - `ahp9`
  - `dawidniescier`
  - `osk`
  - `polarparsnip`
  - `sturla-freyr`

Skila má eins oft og þið viljið þar til skilafrestur rennur út.

## Einkunn

Leyfilegt er að ræða, og vinna saman að verkefni en **skrifið ykkar eigin lausn**. Ef tvær eða fleiri lausnir eru mjög líkar þarf að færa rök fyrir því, annars munu allir hlutaðeigandi hugsanlega fá 0 fyrir verkefnið.

Ef stórt mállíkan (LLM, „gervigreind“, t.d. ChatGTP) er notað til að skrifa part af lausn skal taka það fram. [Sjá nánar á upplýsingasíða um gervigreind hjá HÍ](https://gervigreind.hi.is/).

Sett verða fyrir tíu minni verkefni þar sem átta bestu gilda 5% hvert, samtals 40% af lokaeinkunn.

Sett verða fyrir tvö hópverkefni þar sem hvort um sig gildir 10%, samtals 20% af lokaeinkunn.

> Útgáfa 0.1# verkefni6
