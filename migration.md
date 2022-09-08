# Migration

## Security and privacy

### People

People shouldn't be made publicly available via SPARQL endpoint, but their pages can be viewable individually.

Organisations is not affected by this.

## Denaturing location of TERN assets

## Sites

Ecosystem processes sites are not the same as AusPlots sites. They are only by having the same parent sample, aka. SuperSite.

| Spreadsheet column    | Previous RDF                                           | New RDF                                                                                                     |
| --------------------- | ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| `name`                | `rdfs:label`                                           | `skos:prefLabel`                                                                                            |
| `persistent_uri`      |                                                        |                                                                                                             |
| `ecoimage_name`       | `dcterms:identifier` with datatype `tern:ecoimageName` | Remove and use `rdfs:label` - this is mapped to an identifier when it is being used as a label in EcoImages |
| `internal_identifier` | `alic`                                                 |

Sites need to be classified by type e.g., Ecosystem Processes
