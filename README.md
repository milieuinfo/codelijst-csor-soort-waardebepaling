# Codelijst CSOR — Soort Waardebepaling

Codelijst voor het **Chemische Stoffen en Omgevingsparameters-Register (CSOR)** die de toegelaten soorten waardebepaling definieert.

## Beschrijving

Een soort waardebepaling beschrijft de manier (of de groep van compatibele manieren) waarop een waarde wordt toegekend voor de observatie van het geobserveerde kenmerk. Verschillende soorten waardebepaling leveren fundamenteel andere resultaten op en zijn daardoor onderling onvergelijkbaar.

De codelijst is gepubliceerd als een SKOS-conceptschema onder de namespace van het Departement Omgeving, Vlaanderen.

**Concept scheme URI:**
`https://data.omgeving.vlaanderen.be/id/conceptscheme/csor/soortwaardebepaling`

**Named graph (Virtuoso):**
`https://data.omgeving.vlaanderen.be/id/graph/codelijst-csor-soort-waardebepaling`

## Beschikbare formaten

De codelijst wordt aangeboden in de volgende RDF-formaten:

| Formaat | Bestand |
|---------|---------|
| Turtle (`.ttl`) | `soortwaardebepalingen.ttl` |
| JSON-LD (`.jsonld`) | `soortwaardebepalingen.jsonld` |
| N-Triples (`.nt`) | `soortwaardebepalingen.nt` |
| RDF/JSON (`.rj`) | `soortwaardebepalingen.rj` |

De bestanden bevinden zich in:
```
src/main/resources/be/vlaanderen/omgeving/data/id/conceptscheme/csor/soortwaardebepaling/
```

## Structuur

Elk concept heeft de volgende eigenschappen:

- `skos:prefLabel` — de Nederlandse benaming (bv. `"totaal"`)
- `skos:notation` / `csor:symbool` — het afkortingssymbool (bv. `"TOT"`)
- `skos:definition` — optionele toelichting
- `owl:deprecated` — geeft aan of het concept nog actief is

**Voorbeelden van concepten:**

| Symbool | Label |
|---------|-------|
| `STD` | standaard |
| `TOT` | totaal |
| `OPG` | opgelost |
| `FILT` | gefilterd |
| `GAS` | enkel gasvormig |
| `VLU` | vluchtig |
| `ANORG` | anorganisch |
| `ORG` | organisch |
| `96EC` | EC50 (96h) |
| `48LC` | LC50 (48h) |
| `ZW` | na Zahn Wellens |

## Gebruikte ontologieën

- [SKOS](http://www.w3.org/2004/02/skos/core#) — voor de thesaurusstructuur
- [OWL](http://www.w3.org/2002/07/owl#) — voor deprecatie
- [CSOR-ontologie](https://data.omgeving.vlaanderen.be/ns/csor#) — voor `csor:SoortWaardebepaling` en `csor:symbool`

## Licentie

Dit project valt onder de [GNU General Public License v3.0](LICENSE).
