[![.github/workflows/openapi_check.yaml](https://github.com/bundesAPI/travelwarning-api/actions/workflows/openapi_check.yaml/badge.svg)](https://github.com/bundesAPI/travelwarning-api/travelwarning-api/actions/workflows/openapi_check.yaml)

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

## Änderungen

### version 1.0.1 (September 2021)

* `content` (-> Details des Reise- und Sicherheitshinweis) wurde von [`/travelwarning`](#operations-default-getTravelwarning)
entfernt -> bitte ab jetzt [`/travelwarning/{contentId}`](#operations-default-getSingleTravelwarning) nutzen um `content` abzufragen