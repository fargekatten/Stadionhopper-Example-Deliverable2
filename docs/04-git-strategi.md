# 4. Git-strategi for Stadionhopper

## 4.1 Formål

Versjonskontroll skal brukes som et organiserings- og kvalitetssikringsverktøy, ikke bare som lagring av filer. For et team som skal utvikle Stadionhopper er det viktig at arbeidsflyten er tydelig, at oppgaver er delbare, og at det er mulig å følge hva som er gjort, hva som er i arbeid og hva som er ferdig.

GitHub skal derfor brukes som en felles plattform for:

- oppgaveadministrasjon
- samarbeid
- dokumentasjon
- kodehåndtering
- kvalitetssikring

## 4.2 Arbeidsflyt

Vi anbefaler en enkel og praktisk arbeidsflyt:

1. Opprett en issue for hver større oppgave eller forbedring.
2. Opprett en egen feature-branch fra `main`.
3. Løs oppgaven lokalt eller i branch.
4. Lag minst ett commit per logisk del av arbeidet.
5. Opprett pull request når oppgaven er ferdig.
6. Gjennomgå kode og dokumentasjon sammen med minst ett annet medlem.
7. Merge til `main` når godkjenning er gitt.

Dette gir både tydelig sporbarhet og lav risiko for at store endringer blir løftet inn i hovedbranchen uten gjennomgang.

## 4.3 Branchingstrategi

Vi anbefaler denne modellen:

- `main` – produksjonsklar hovedlinje
- `feature/<kort-navn>` – for nye funksjoner eller dokumentasjonsarbeid
- `fix/<kort-navn>` – for feilrettinger
- `docs/<kort-navn>` – for dokumentasjonsoppgaver

Eksempler:

- `feature/login-flow`
- `feature/match-overview`
- `docs/architecture-deliverable`
- `fix/checkin-validation`

Denne modellen er enkel, men tydelig. Den gjør det lett å holde `main` ryddig og samtidig mulig å jobbe parallelt.

## 4.4 Pull requests

En pull request skal være ment som et kvalitetssikringsverktøy. Før merge bør PR-en inneholde:

- kort beskrivelse av hva som er endret
- hva problemet løser
- hvilke tester som er kjørt
- eventuelle avhengigheter eller risikoer

Det bør også være mulig å legge ved screenshots eller wireframes hvis det er relevant for visuell utvikling.

For dette prosjektet er det spesielt viktig at dokumentasjon, UX og arkitektur blir gjennomgått i PR-en fordi disse delene er sentrale for eksamensoppgaven.

## 4.5 Kodegjennomganger

Alle PR-er skal gjennomgås av minst ett annet gruppemedlem. Kodegjennomgang skal fokuseres på:

- korrekthet
- lesbarhet
- sammenheng med krav
- teknisk kvalitet
- dokumentasjon

Dette er viktig fordi det styrker helheten i prosjektet, ikke bare individuelle funksjoner.

## 4.6 CI/CD-strategi

Selv om dette ikke nødvendigvis trenger å være implementert i første versjon, er det viktig å ha en plan:

### Automatiske bygg
- hver pull request skal trigge en bygg
- GitHub Actions skal sørge for at prosjektet kan kompilers / bygges

### Automatiske tester
- unit tests for logikk
- integration tests for API og datalagring
- UI-tests for viktig brukerflyt

### Kvalitetskontroller
- linting
- formattering
- sikkerhetskontroll på avhengigheter
- statisk analyse om dette er relevant

### Leveransepipeline
- kode merges til `main`
- CI kjøres
- tester gjennomføres
- dersom alt er grønt oppdateres produktet eller en demo-miljø

## 4.7 Dokumentasjon som del av Git-flow

I denne oppgaven er dokumentasjonsarbeidet et kritisk element. Derfor bør dokumentasjon også være innlemmet i Git-flowen:

- nye dokumentkapitler i egne branches
- PR for dokumentasjon
- godkjenning før merge

Dette er spesielt relevant fordi oppgaven eksplisitt krever at dokumentasjon og teknisk spor er publisert og tilgjengelig i Git.

## 4.8 Praktisk eksempel

Eksempel på arbeidsflyt i prosjektet:

- `docs/domain-model` – oppdateres etter gruppering av domenemodell
- `feature/login-form` – håndterer påloggingsflyt
- `feature/stadium-map` – kart og stadionvisning
- `docs/git-strategy` – dokumentasjon av arbeidsflyten

Dette gjør at dokumentasjon og utvikling blir håndtert parallelt, og at alle endringer sporbarhet og oppfølging i GitHub.

## 4.9 Oppsummering

Git-strategien skal være enkel, tydelig og praktisk. Målet er ikke å bygge den mest avanserte arbeidsflyten, men å sikre at teamet kan samarbeide uten kaos. En vellykket Git-strategi i Stadionhopper vil være:

- tydelig i branching
- trygg i merge
- gjennomsiktig i pull requests
- integrert med dokumentasjon og kvalitetssikring

Dette er også viktig fordi oppgaven krever at teamet viser at de forstår hvordan teknisk arbeid, utviklingsprosesser og dokumentasjon henger sammen.
