# 3. UX og wireframes for Stadionhopper

## 3.1 Hva UX-handler her?

UX er ikke bare hvordan appen ser ut. UX handler om hvordan brukeren forstår systemet, hvordan de navigerer, hvilken informasjon som er viktig først, og hvor de får den minste motstanden i å oppnå et mål. For Stadionhopper er det avgjørende å ha en brukerreise som er enkel, tydelig og motiverende.

Målet er å redusere den mentale byrden for brukeren:

- finne en kamp
- forstå hvor den er
- oppdage om det er interessant
- registrere at man har vært der
- se tilbake på tidligere opplevelser

Hvis brukerflyten er enkel, blir systemet både mer brukbart og mer sannsynlig for å bli brukt igjen.

## 3.2 Brukerbehov som styrer UX

Basert på målgruppen og produktvisjonen, er de viktigste brukerbehovene:

- rask tilgang til kommende kamper
- enkel bruk uten mye læring
- tydelig plassering av kamp og stadion
- personlig historikk som gjør opplevelsen verdifull
- minimum av friksjon ved innsjekking

Dette peker mot et design hvor informasjon er prioritet, mens sosiale og gamificerende elementer er sekundære i første iterasjon.

## 3.3 UX-prinsipper for Stadionhopper

### 1. Vis kampinformasjon først
Det mest kritiske elementet er å vise relevante kamper raskt. Derfor må landing page eller “kampoversikt” være tydelig og visuell.

### 2. Reduser antall klikk
Brukeren skal kunne gå fra oversikt til detalj til innsjekking med så få trinn som mulig.

### 3. Prioritér tydelig visuell kode
Kampkort, dato, tid, lag, stadium og “registrer besøk” skal være umiddelbart synlig.

### 4. Historikk som motivasjonsmekanisme
Den personlig historikken er viktig, fordi den skaper verdi over tid og gjør appen mer enn en kampoversikt.

### 5. Visuelt tydelig flyt fra oppdagelse til opplevelse
Dette er viktig fordi produktet skal gi brukeren en følelse av progresjon: finne – oppleve – lagre – gjenoppleve.

## 3.4 Wireframes

### Wireframe 1: Pålogging

```text
+--------------------------------------+
| Stadionhopper                        |
|--------------------------------------|
| E-post/email                         |
| Passord                             |
| [Logg inn]                          |
| [Opprett bruker]                    |
| Har du glemt passord?               |
+--------------------------------------+
```

Dette designet er valgt fordi det er enkelt, raskt og godt forbrukerforståelig. Pålogging er en kritisk funksjon, men den skal ikke ta fokus bort fra hovedverdien i appen.

### Wireframe 2: Kampoversikt / landing page

```text
+--------------------------------------+
| Stadionhopper     Søk | Kategori    |
|--------------------------------------|
| KAMPER                              |
|--------------------------------------|
| [Kampkort]                          |
| 12. okt 19:00                       |
| Molde FK - Aalesund FK             |
| Åråsen Stadion                     |
| [Se kamp] [Registrer besøk]        |
|--------------------------------------|
| [Kampkort]                          |
| 15. okt 18:00                       |
| Kristiansund - Ranheim             |
| Nordmøre Arena                    |
| [Se kamp] [Registrer besøk]        |
+--------------------------------------+
```

Det sentrale her er at kampkortene er korte, informative og lette å skanne. Dette gjør løsningen godt egnet for bruk på mobil.

### Wireframe 3: Kampdetalj

```text
+--------------------------------------+
| Tilbake | Kampdetaljer             |
|--------------------------------------|
| Molde FK vs Aalesund FK             |
| 12. okt 19:00                       |
| Åråsen Stadion                      |
| Adresse: ...                        |
|--------------------------------------|
| Oppsummering: 18.000 forventede     |
| Klima: Sol, 14°C                    |
| [Registrer besøk]                   |
| [Vis på kart]                       |
+--------------------------------------+
```

Dette designet gjør at fokus ligger på hva brukeren trenger for å ta en beslutning. Her blir det tydelig at systemet ikke bare er en liste; det er også et verktøy for planlegging og beslutningstaking.

### Wireframe 4: Profil / historikk

```text
+--------------------------------------+
| Profil        Historikk             |
|--------------------------------------|
| Navn: Oda                        |
| Favorittklubb: Molde FK           |
| Besøkte kamper: 14                 |
|--------------------------------------|
| 12. okt | Molde FK - Aalesund FK |
| 25. sep | Kristiansund - Ranheim |
| 08. sep | MFK - Tromsdalen         |
| [Se alle]                          |
+--------------------------------------+
```

Historikken er viktig fordi den skaper langsiktig verdi. Den gjør at Stadionhopper blir mer enn et “kampkart”; det blir et sted hvor brukeren samler opplevelser.

### Wireframe 5: Stadionkart / oppdagelse

```text
+--------------------------------------+
| Stadioner            [Kart / Liste] |
|--------------------------------------|
| [Kartvisning med punkter]           |
| 1: Åråsen Stadion                   |
| 2: Nordmøre Arena                   |
| 3: Karmøy Stadion                   |
| [Filtrer: Møre og Romsdal]         |
+--------------------------------------+
```

Kartet er viktig fordi det kobler kampinformasjon til sted, og er en logisk måte å oppdage nye stadioner på.

## 3.5 Designvalg og begrunnelse

### Enkelt, mobilvennlig design
Stadionhopper skal være et “siste-mile” produkt som brukes når brukeren aktivt vil finne eller registrere en kamp. Det betyr at vi prioriterer mobilvennlighet og enkel navigasjon over estetikk eller kompleks funksjonalitet.

### Tydelig kampoversikt som hovedfokus
Brukere må raskt forstå hvilke kamper som finnes og hva som er relevant. Derfor kommer oversiktssiden først.

### Historikk som langsiktig verdi
Mange løsninger stopper på “kampoversikt”. Stadionhopper blir annerledes fordi brukeren får verdi over tid ved å samle opplevelser og bygge historikk.

### Redusert fokus på sosialt innhold i første iterasjon
Selv om sosial interaksjon er viktig i produktvisjonen, er dette ikke det første brukeren trenger. For å sikre god brukbarhet i MVP-en må vi fokusere på kjernereisene først.

## 3.6 Brukerflyt

Den sentrale brukerflyten er:

1. Brukeren åpner appen
2. Brukeren ser kommende kamper
3. Brukeren velger en kamp
4. Brukeren ser kampdetaljer og stadion
5. Brukeren registrerer besøket
6. Brukeren får opp historikk og opplevelse

Dette er både enkel og målrettet. Den skaper verdi for brukeren uten å måtte ta i bruk uklar eller kompleks funksjonalitet alt for tidlig.

## 3.7 Oppsummering

UX-en i Stadionhopper bør være rettet mot tre mål:

- gjøre oppdagelse av lokale kamper enklere
- gjøre planlegging av besøk raskere
- sørge for at brukerens historikk blir en motivasjonsfaktor

Wireframes og brukerflyt viser at dette kan oppnås uten å være alt for kompleks. Et enkelt, tydelig og målrettet design er i tråd med både brukerbehov og eksamenskrav.
