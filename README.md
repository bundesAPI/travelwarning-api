[![.github/workflows/openapi_check.yaml](https://github.com/bundesAPI/travelwarning-api/actions/workflows/openapi_check.yaml/badge.svg)](https://github.com/bundesAPI/travelwarning-api/actions/workflows/openapi_check.yaml)

# Auswärtiges Amt OpenData Schnittstelle

Enthält die [Beschreibung](https://travelwarning.api.bund.dev/index.html) für die Schnittstelle zum Zugriff auf die Daten
des [Auswärtigen Amtes](https://www.auswaertiges-amt.de/de/) im Rahmen der
[OpenData](https://www.auswaertiges-amt.de/de/open-data-schnittstelle/736118) Initiative.

## Deaktivierung

Die Schnittstelle kann deaktiviert werden, in dem Fall wird ein leeres JSON-Objekt zurückgegeben.

## Fehlerfall

Im Fehlerfall wird ein leeres JSON-Objekt zurückgegeben.

## Nutzungsbedingungen

Die Nutzungsbedingungen sind auf der [OpenData-Schnittstelle](https://www.auswaertiges-amt.de/de/open-data-schnittstelle/736118)
des Auswärtigen Amtes zu finden.

## Änderungen [(offizielles Changelog)](https://www.auswaertiges-amt.de/de/-/2412916)

### version [1.2.7](https://www.auswaertiges-amt.de/de/-/2412916) - (02.08.2022)

Dreistellige ISO-Ländercodes ([ISO 3166-1 alpha-3](https://de.wikipedia.org/wiki/ISO-3166-1-Kodierliste)) wurden als `iso3CountryCode` hinzugefügt.

### version [1.2.6](https://www.auswaertiges-amt.de/de/-/2412916) - (08.12.2021)

Es werden zusätzlich zu jedem Land **Ländercodes** mit jeweils **zwei Buchstaben** mit ausgegeben.

Die Länderkürzel werden bei [`/travelwarning`](https://travelwarning.api.bund.dev/#operations-default-getTravelwarning) und [`/travelwarning/{contentId}`](https://travelwarning.api.bund.dev/#operations-default-getSingleTravelwarning) in einem neuen Attribut ausgegeben z.B. in: [`/travelwarning/199124`](https://www.auswaertiges-amt.de/opendata/travelwarning/199124).

### version [1.2.5](https://www.auswaertiges-amt.de/de/-/2412916) (ursprünglich geplant für Ende September 2021)

`content` (-> Details des Reise- und Sicherheitshinweis) wurde von [`/travelwarning`](https://travelwarning.api.bund.dev/#operations-default-getTravelwarning)
entfernt -> bitte ab jetzt [`/travelwarning/{contentId}`](https://travelwarning.api.bund.dev/#operations-default-getSingleTravelwarning) nutzen um `content` abzufragen

`flagURL` (-> Flaggen der Länder) wurde entfernt.
