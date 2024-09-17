# Java for lærlinger
Ressurser og tips for å lære og bruke Java

## Generere et tomt Java-prosjekt med oppdatert Maven-oppsett (Java 22)

#### 1. Endre verdiene `-DgroupId`, `-DartifactId` og `-Dversion` med dine egne prosjekt-detaljer. Disse tre verdiene er påkrevd.

| Felt          | Anbefalte verdier        |
|-------------- |-----------------|
| groupId       | Anbefales å bruke en domene-adresse, feks din arbeidsgiver eller ditt eget domene. Dersom du jobber i NAV vil det være "no.nav". Jobber du i SPK vil det være "no.spk" osv. GruppeId'en gjenspeiler ofte hvilken organisasjon som eier prosjektet.|
| artifactId    | Dette er navnet på programmet du ønsker å lage. Anbefales å skrive enten ett enkelt navn (feks "javaprosjekt") eller et navn med bindestrek (feks "olas-javaprosjekt"). Dersom du feks lager spillet Tre-På-Rad, kan navnet være "tre-paa-rad".  |
| version       | Anbefales å la feltet stå som "1.0.0". Denne verdien kan du også endre senere i kode-editoren din. |

#### 2. Verdiene `archetypeGroupId`, `archetypeArtifactId` og `archetypeVersion` skal ikke endres og må være som de er.

Eksempel:

```shell
mvn archetype:generate -DarchetypeGroupId=no.dervis \
                    -DarchetypeArtifactId=java-starter \
                    -DarchetypeVersion=1.0.12 \
                    -DgroupId=no.nav \
                    -DartifactId=javaprosjekt \
                    -Dversion=1.0.0 \
                    -DjdkVersion=22 \
                    -DjavaPreviewFeatures=yes \
                    -DinteractiveMode=false
```
