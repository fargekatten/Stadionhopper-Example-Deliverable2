# 5. Teststrategi for Stadionhopper

## 5.1 Formål med teststrategien

Kvalitetssikring er ikke et tillegg til utviklingen; det er en integrert del av prosessen. Stadionhopper skal bygges i steg, og derfor må vi ha en teststrategi som sikrer at produktet utvikler seg mot de overordnede målene: brukbarhet, pålitelighet og forståelig teknisk løsning.

Teststrategien skal derfor håndtere:

- om koden virker som forventet
- om brukerflyten er forståelig
- om viktige krav blir validert
- om systemet kan utvikles videre uten at kvaliteten går ned

## 5.2 Testnivåer

### 5.2.1 Enhetstester
Enhetstester fokuserer på små logiske enheter, for eksempel:

- validering av brukerdata
- beregning av dato eller kampstatus
- filtrering av kamper etter område eller dato
- logikk for innsjekking

Disse testene skal være raske og være ansvarlig for at enkel logikk fungerer korrekt.

### 5.2.2 Integrasjonstester
Integrasjonstester må sikre at delene av systemet fungerer sammen, for eksempel:

- frontend henter kampdata fra backend
- brukerprofil oppdateres når innsjekking legges til
- kampdata hentes og vises korrekt i oversikten
- database og service-lag kommuniserer som forventet

Dette er spesielt viktig når systemet utvikles i flere moduler og flere teammedlemmer jobber samtidig.

### 5.2.3 Akseptansetester
Akseptansetester verifiserer at systemet oppfyller brukerkrav. Eksempler:

- en bruker kan finne en kamp
- en bruker kan registrere at de har vært på kampen
- en bruker kan gå tilbake og se historikken sin
- en bruker kan logge inn og få tilgang til personlig historikk

Akseptansetester er viktig for eksamen fordi de viser at vi tester på kravnivå, ikke bare på teknisk implementasjonsnivå.

## 5.3 Testansvar

For å gjøre testarbeidet tydelig bør teamet ha ansvar for ulike deler:

- Frontend-utvikler: brukerflyt og visuell test
- Backend-utvikler: logikk og integrasjon
- Dokumentasjon / prosjektleder: kvalitetssikring av krav og testdekning

Dette gjør at særlig viktige brukerflyter blir gjennomgått systematisk, og at ansvaret ikke ligger på ett enkelt medlem.

## 5.4 Kvalitetskriterier

For at en versjon kan bli godkjent bør den oppfylle disse kriteriene:

- funksjonelle krav er oppfylt
- viktig brukerflyt er testet
- det finnes ingen kritiske feil i hovedflyten
- dokumentasjon er oppdatert
- endringene er gjennomgått i pull request

Dette er et viktig kvalitetsnivå fordi prosjektet ikke bare skal ha fungerende kode, men også et samlet og forståelig teknisk grunnlag for videre arbeid.

## 5.5 Testplan for Stadionhopper

### Første iterasjon
- enhetstest av kampfiltrering
- enhetstest av innlogging/validering
- integrasjonstest av oppslag av kampoversikt
- akseptansetest av “finne og registrere kamp”

### Andre iterasjon
- test av historikk og profilvisning
- test av kart- og stadionvisning
- test av sosial interaksjon om denne utvikles

## 5.6 CI/CD som kvalitetssikring

Automatisert kvalitetssikring bør være en del av prosessen:

- bygg på PR
- kjør test-suite ved hver merge
- stopp merge hvis kritiske tester feiler
- enkle rapporter om testdekning og kvalitet

Dette viser at teamet ikke bare skriver tester etterpå, men faktisk flytter kvalitet inn i arbeidsflyten.

## 5.7 Oppsummering

Teststrategien for Stadionhopper bør være enkel, men struktureret. Vi må teste på flere nivåer:

- logikk
- integrasjon
- brukerflyt
- kravoppfyllelse

Det er spesielt viktig å teste hovedflyten, fordi dette er der produktverdien ligger. Hvis brukeren kan oppdage en kamp, gå til detalj, registrere et besøk og se historikken, så har vi et godt grunnlag for videreutvikling.
