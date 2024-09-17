# Java for lærlinger
Ressurser og tips for å lære og bruke Java

## Generere et tomt Java-prosjekt med oppdatert Maven-oppsett (Java 22)

1. Endre verdiene `-DgroupId`, `-DartifactId` og `-Dversion` med dine egne prosjekt-detaljer. Disse tre verdiene er påkrevd.

| Felt          | Anbefalte verdier        |
|-------------- |-----------------|
| groupId       | Bruk domene-adressen til din arbeidsgiver. Dersom du jobber i NAV vil det være "no.nav". Jobber du i SPK vil det være "no.spk" osv.|
| artifactId    | Dette er navnet på programmet du ønsker å lage.  |
| version       | Anbefales å la feltet stå som "1.0.0". Denne verdien kan du også endre senere i kode-editoren din. |

2. Verdiene `archetypeGroupId`, `archetypeArtifactId` og `archetypeVersion` skal ikke endres og må være som de er.

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
