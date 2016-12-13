# SBVR
## Bedoeling:
Samenbrengen van resources en proberen alle info die de presentatie-makers nodig hebben te verzamelen en eventueel al (gedeeltelijk) verwerken.

## Resources:
In order of perceived usefulness:
* PDF file in deze dir.
* [Zeer goed uitleggende presentatie over SBVR](http://www.buildingbusinesscapability.com/presentations/2014/1658.pdf)
* [Presentatie over SBVR](http://knut.hinkelmann.ch/lectures/ISA2010/ISA-7-SBVR.pdf)
* [Tutorial over SBVR](http://www.kdmanalytics.com/sbvr/sbvr_intro_1.html)
* [Tutorial over gebruik van SBVR in een programma](http://loki.ia.agh.edu.pl/wiki/docs:sbvr-tutorial) Niet echt handig voor standaard zelf maar kan de standaard wel beter verstaanbaar maken.
* [Lange presentatie over SBVR](http://www.businesssemantics.com/Resources/How_SBVR_Adds_Knowledge_Richness_to_ISO_TC_37_Terminology_Standards.pdf) Zonder orale uitleg misschien niet zo heel duidelijk wat er in deze presentatie staat?

## Linken met cursus
* Van voorbeeldzin zoals: `it is obligatory that each rental has at least one driver`, een link leggen naar een UML schema, en dat linken aan het documenteren van functionele vereisten vanuit het dataperspectief (Zie semestertaak: datamodel).
* Van voorbeeldzin zoals: `Cars are serviced at 5.000 miles intervals` een link leggen naar OCL

## Voorbeeldzinnen
* `it is necessary that each __match__ has at least one __game__`
  * Kan ook obligatory zijn ipv necesarry, hangt er van af of het per definitie waar is, of dat het waar zou moeten zijn omdat wij er voor moeten zorgen dat het waar is. Wat er nu staat dat het per definite klopt.
* `it is obligatory that each __team__ has exactly five __Starter players__`
* `it is obligatory that each __team__ has exactly one __Reserve player__`


## Voorbeeld definities
BELANGRIJK: Gebruik juiste font styling, want dat is hoe SBVR structured english is, gewoon engels met font styling.


Definitie van __Player__

```
__Player__
    Definition:         A __person__ who plays for a __team__

__Player__ has __playerID__
    Necessity:          Each __Player__ has exactly one __playerID__
    
__Player__ has __name__
    Necessity:          Each __Player__ has exactly one __name__
    
__Player__ has __role__
    Necessity:          Each __Player__ has at least one at most two __roles__
    
__Player__ has __sumonnerName__
    Necessity:          Each __Player__ has exactly one __sumonnerName__
```

Definitie van een relatie:
    
```    
__Player__ plays for __Team__
    Synonymous Form:    __Team__ owns __Player__
    Definition:         __Player__ has a contract with __Team__

```
