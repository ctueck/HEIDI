# HEI Identifiers Whitepaper

## Relevance

Higher education institutions (HEIs) are a pivotal enitity for many different systems and applications. Institutional identifiers are thus a matter of priority.

With less than 10000 HEIs in Europe the numbers are relatively managable, but yet large enough to warrant some standardisation to allow for data exchange without manual intervention or mapping.

## Existing systems

Various approaches already exist to identify higher education institutions in Europe:

| Identifier               | Maintained by         | Used in                | Link                                                                      | Comment                                              |
|:-------------------------|:----------------------|:-----------------------|:--------------------------------------------------------------------------|:-----------------------------------------------------|
| PIC                      | EU                    | EU programmes, European Student Card | [EU portal](https://ec.europa.eu/info/funding-tenders/opportunities/portal/screen/how-to-participate/participant-register) |     |
| Erasmus Institution Code | EU                    | Erasmus+               | [EU page](https://eacea.ec.europa.eu/erasmus-plus/actions/erasmus-charter_en)   |                                                |
| eIDAS identifier         | EU                    | EDCI                   | [EU page](https://ec.europa.eu/digital-single-market/en/trust-services-and-eid) | Just an organisational identifier. Not HE specific   |
| SCHAC                    | Géant                 | ELMO, Emrex, EWP       | [SCHAC](https://wiki.refeds.org/display/STAN/SCHAC)                       |                                                      |
| ETER ID                  | EU-funded consortium  | ETER, OrgReg, DEQAR    | [ETER](https://eter-project.com/#/home)                                   |                                                      |
| DEQARINST ID		   | EQAR		   | DEQAR		    | [DEQAR data set](https://www.eqar.eu/qa-results/get-data/download-data-sets/) | main need for HEIs not contained in ETER         |

The [EWP Registry Service](https://github.com/erasmus-without-paper/ewp-specs-api-registry/#registry-service) provides an accessible mapping between SCHAC, PIC and Erasmus codes for a number, but not all HEIs in Europe. The EU provides a [spreadsheet](https://eacea.ec.europa.eu/erasmus-plus/actions/erasmus-charter_en) of Erasmus Institution Codes, including the related PIC code.

Given that each organisation has their own approach how to deal with demographic changes (e.g. mergers), there is not necessarily a one-to-one relationship between different identifiers.

In conclusion, existing identifiers for HEIs in Europe are currently not fully articulated to each other.

## Use Cases
Placeholder to insert use cases from stakeholders.

## Requirements

- unique
- stable over time
- track demography & history (e.g. mergers, name changes, ...)

## Options

1. Agreement on one system
    - Could we agree on one? Which one?
    - Who maintains it?
2. One or several systems to provide mapping/link
    - Who could offer it?
    - How to propagate changes? Risk of inconsistencies?
3. Institutions to publish their identifiers
    - How to ensure critical mass?
    - How to discover institution's list?
4. Additional mapping/translation service
    - Who would run it?
    - Maybe highest overhead of all options

