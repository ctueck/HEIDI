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

The following use cases should be made possible/be facilitated by an enhanced approach to HEI identifiers.

**NB: This is an initial collection of use cases. We aim to supplement those with contributions from stakeholders during the discussion. Use cases should be defined in line with [this template](../Supporting/UseCaseTemplate.md).**

### Cross-check Institution Data

**Users:** HEIs, recognition offices, students, employers

The users receives data from or about a HEI, and wishes to automatically search another database for additional data about the HEI concerned.

For example, the user might recieve student mobility data, such as a transcript of records, via EMREX or EWP, or a qualification from a student applying for recognition. The user wants to acquire information on the sending institution's quality assurance status from DEQAR.

### Populate EDCI Accreditation Database

**Users:** national authority

The authority wants to populate the Accreditation Database for Europass Digital Credentials with data on quality-assured HEIs that is already available in DEQAR.

### Correlate Datasets

**Users:** researchers, policy makers, statistics offices

The user has data on HEIs in Europe and wishes to correlate this with other data or statistics, e.g. from ETER.

## Requirements

To be derived from use cases and discussed at first meeting.

## Options

To be formulated in generic terms and then discussed at first meeting.

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

