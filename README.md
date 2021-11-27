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

### version [1.2.5](https://www.auswaertiges-amt.de/de/-/2412916) (ursprünglich geplant für Ende September 2021)

*Einführung verzögert sich*

`content` (-> Details des Reise- und Sicherheitshinweis) wurde von [`/travelwarning`](#operations-default-getTravelwarning)
entfernt -> bitte ab jetzt [`/travelwarning/{contentId}`](#operations-default-getSingleTravelwarning) nutzen um `content` abzufragen

`flagURL` (-> Details des Reise- und Sicherheitshinweis) ist noch (Ende November 2021) präsent soll aber zukünftig entfernt werden -> es werden keine **Flaggen** mehr angeboten

