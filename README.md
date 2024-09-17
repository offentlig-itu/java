# Java for lærlinger
Ressurser og tips for å lære og bruke Java

## Generere et tomt Java-prosjekt med oppdatert Maven-oppsett (Java 22)

1. Endre verdiene `-DgroupId`, `-DartifactId` og `-Dversion` med dine egne prosjekt-detaljer. Disse tre verdiene er påkrev.

| Felt          | Eksempel        |
|-------------- |-----------------|
| groupId       |                 |
| artifactId    |                 |
| version       |                 |

2. Verdiene `archetypeGroupId`, `archetypeArtifactId` og `archetypeVersion` skal ikke endres og må være som de er.

Eksempel:

```shell
mvn archetype:generate -DarchetypeGroupId=no.dervis \
                    -DarchetypeArtifactId=java-starter \
                    -DarchetypeVersion=1.0.12 \
                    -DgroupId=org.nav \
                    -DartifactId=javaprosjekt \
                    -Dversion=1.0.0 \
                    -DjdkVersion=22 \
                    -DjavaPreviewFeatures=yes \
                    -DinteractiveMode=false
```
