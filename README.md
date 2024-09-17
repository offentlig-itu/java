# Java for lærlinger
Ressurser og tips for å lære og bruke Java

## Generere et tomt Java-prosjekt med oppdatert Maven-oppsett (Java 22)

```shell
mvn archetype:generate -DarchetypeGroupId=no.dervis \
                    -DarchetypeArtifactId=java-starter \
                    -DarchetypeVersion=1.0.12 \
                    -DgroupId=org.mygroup \
                    -DartifactId=demoapp \
                    -Dversion=1.0.0 \
                    -DjdkVersion=22 \
                    -DjavaPreviewFeatures=yes \
                    -DinteractiveMode=false
```
