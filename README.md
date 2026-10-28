# EiendelsBuddy – offentlig appinformasjon

Dette repoet inneholder bare offentlig appbeskrivelse, personvernerklæring og
bruksvilkår for EiendelsBuddy og GoogleAPIApp. Appkode, konfigurasjon, token,
databaser og dokumenter skal aldri legges her.

## Publisering

GitHub Pages publiserer `main` fra rotmappen. Siden er statisk HTML/CSS og
krever ingen byggeprosess eller avhengigheter. `.nojekyll` slår av Jekyll.

Forventet adresse: https://smellyglove.github.io/eiendelsbuddy-info/

## Google Auth Platform

På Branding-siden:

| Felt | Verdi |
| --- | --- |
| Application home page | `https://smellyglove.github.io/eiendelsbuddy-info/` |
| Application privacy policy link | `https://smellyglove.github.io/eiendelsbuddy-info/personvern/` |
| Application terms of service link | `https://smellyglove.github.io/eiendelsbuddy-info/vilkar/` |
| Authorized domains | `smellyglove.github.io` |

Lagre, gå til Audience og forsøk Publish app. Dette endrer OAuth-prosjektets
publiseringsstatus, uten å gjøre den lokale applikasjonen offentlig.
Etter overgang til In production må brukeren autorisere GoogleAPIApp på nytt
for å erstatte en innlogging utstedt i Testing.

Hvis Google krever eierskapsbekreftelse: legg til nettsiden som en
URL-prefix-property i Google Search Console med prosjektets eierkonto.
Den kontospesifikke HTML-filen eller metataggen Google gir, kan publiseres
her. Ikke bruk en tilfeldig bekreftelseskode eller legg inn OAuth-hemmeligheter.

Publisering hos Google og ny autorisering er separate, manuelle steg. En
vellykket GitHub Pages-deploy beviser ikke at Google har godtatt oppsettet.
