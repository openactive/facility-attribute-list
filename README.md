# Facility Attribute List

> Status: Draft | [Please Provide Feedback via GitHub](https://github.com/openactive/facility-attribute-list/issues)

## Status

This list is in a draft state, however every effort will be made in subsequent revisions to maintain the IDs associated with the concepts enumerated here.

## Documentation

This repository holds the [JSON-LD definition](https://openactive.io/facility-attribute-list/facility-attribute-list.jsonld) of the OpenActive Facility Attribute List controlled vocabulary.

This controlled vocabulary MUST be referenced within a `Concept` via `inScheme` using the URL `"https://openactive.io/facility-attribute-list"` (which will return the [JSON-LD definition](https://openactive.io/facility-attribute-list/facility-attribute-list.jsonld) if the `Accept` header contains `application/ld+json`).

This controlled vocabulary SHOULD be retrieved frequently using an HTTP GET and cached within an application, to ensure that the most up-to-date version is displayed to the user, while also protecting against network failure when accessing the underlying resource. To access this controlled vocabulary the application MUST GET the URL `"https://openactive.io/facility-attribute-list/facility-attribute-list.jsonld"` (note there is no www in the URL) which does not require a specific `Accept` header, and is cached via CDN. The controlled vocabulary is also available via a GET of the URL `"https://openactive.io/facility-attribute-list"` using an `Accept` header of `application/ld+json`, for completeness, however this shorter URL MUST NOT be used in production.

Please raise requests for content or issues related to this controlled vocabulary via [GitHub](https://github.com/openactive/facility-attribute-list/issues). 

## Example use

The example below illustrates an `"beta:facilityAttribute"` property for an `FacilityUse` that describes a 3G Artificial Grass pitch.

```json
"beta:facilityAttribute": [
  {
    "type": "Concept",
    "id": "https://openactive.io/facility-attribute-list#8c4ba90c-2ceb-4a38-aeba-1875da03c227",
    "prefLabel": "Concrete",
    "inScheme": "https://openactive.io/facility-attribute-list"
  }
]
```

## Source data

Please see the [spreadsheet](https://docs.google.com/spreadsheets/d/11jT9e2fzmIXHPrxm6zsnjWWUT2q8_Op5ZkRDmi1nYAw/edit) used to generate the JSON-LD representation, comments welcome!


## Licence

The documentation and data in this repository is published under the [Creative Commons CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.

