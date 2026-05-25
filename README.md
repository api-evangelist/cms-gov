# CMS — Centers for Medicare & Medicaid Services (cms-gov)

The Centers for Medicare & Medicaid Services (CMS) is the U.S. federal agency within the Department of Health and Human Services that administers Medicare, Medicaid, the Children's Health Insurance Program (CHIP), the Health Insurance Marketplace, and the broader CMS open-data program. CMS operates one of the largest collections of HL7 FHIR APIs in the U.S. federal government — Blue Button 2.0, BCDA, AB2D, DPC, and the upstream BFD server — alongside the Marketplace API, the data.cms.gov open-data catalog, the Provider Data Catalog, the Quality Payment Program API, and the Medicare Coverage Database.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=government-api-evangelist&utm_content=repo)

## Tags

 - Healthcare, Medicare, Medicaid, FHIR, Bulk Data, Open Data, Government, Federal, Claims, Insurance, ACA, Marketplace, Quality

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### CMS Blue Button 2.0 API

Developer-friendly, OAuth 2.0-enabled HL7 FHIR R4 API delivering Medicare Part A, B, and D claims data for 60+ million beneficiaries after consent. Patient, Coverage, and ExplanationOfBenefit resources.

**Human URL:** [https://bluebutton.cms.gov/developers/](https://bluebutton.cms.gov/developers/)

- [Documentation](https://bluebutton.cms.gov/developers/)
- [Sandbox Explorer](https://bluebutton.cms.gov/api/v2/explorer/)
- [OpenAPI](openapi/cms-gov-blue-button-2-openapi.yml)
- [JSON Schema — ExplanationOfBenefit](json-schema/cms-gov-explanation-of-benefit-schema.json)
- [JSON Schema — Patient](json-schema/cms-gov-patient-schema.json)
- [JSON Schema — Coverage](json-schema/cms-gov-coverage-schema.json)
- [JSON-LD](json-ld/cms-gov-context.jsonld)
- [Naftiko Capability — Blue Button FHIR](capabilities/blue-button-fhir.yaml)

### CMS Beneficiary Claims Data API (BCDA)

Bulk HL7 FHIR (Flat FHIR) export for Medicare Shared Savings Program ACOs. Asynchronous `$export` of Patient, Coverage, and ExplanationOfBenefit as NDJSON.

**Human URL:** [https://bcda.cms.gov/](https://bcda.cms.gov/)

- [Documentation](https://bcda.cms.gov/guide.html)
- [Sandbox](https://sandbox.bcda.cms.gov/)
- [OpenAPI](openapi/cms-gov-bcda-openapi.yml)
- [Naftiko Capability — BCDA Bulk FHIR](capabilities/bcda-bulk-fhir.yaml)

### CMS AB2D API

Bulk HL7 FHIR export for Medicare Part D Prescription Drug Plan sponsors. ExplanationOfBenefit NDJSON for enrolled beneficiaries since 2020.

**Human URL:** [https://ab2d.cms.gov/](https://ab2d.cms.gov/)

- [Documentation](https://ab2d.cms.gov/getting-started/)
- [Swagger UI](https://sandbox.ab2d.cms.gov/swagger-ui/)
- [OpenAPI](openapi/cms-gov-ab2d-openapi.yml)
- [Naftiko Capability — AB2D Bulk FHIR](capabilities/ab2d-bulk-fhir.yaml)

### CMS Data at the Point of Care API (DPC)

Bulk HL7 FHIR delivery of Medicare claims to fee-for-service providers at the point of care. Provider registers Practitioner, Patient, and Group attribution rosters then exports ExplanationOfBenefit, Coverage, and Patient.

**Human URL:** [https://dpc.cms.gov/](https://dpc.cms.gov/)

- [Documentation](https://dpc.cms.gov/docs)
- [OpenAPI](openapi/cms-gov-dpc-openapi.yml)
- [Naftiko Capability — DPC Bulk FHIR](capabilities/dpc-bulk-fhir.yaml)

### CMS Beneficiary FHIR Data Server (BFD)

Upstream HL7 FHIR R4 service that powers Blue Button 2.0, BCDA, AB2D, and DPC. Ingests claims from the CMS Chronic Conditions Warehouse (CCW). Peering-only access via mutual TLS.

**Human URL:** [https://bfd.cms.gov/](https://bfd.cms.gov/)

- [Source Code](https://github.com/CMSgov/beneficiary-fhir-data)
- [OpenAPI](openapi/cms-gov-bfd-openapi.yml)
- [Naftiko Capability — BFD FHIR](capabilities/bfd-fhir.yaml)

### CMS Marketplace API

Qualified Health Plan (QHP) and Stand-alone Dental Plan (SADP) data from healthcare.gov including plan finder, plan compare, rates, benefits, crosswalks, and issuer details.

**Human URL:** [https://developer.cms.gov/marketplace-api/](https://developer.cms.gov/marketplace-api/)

- [OpenAPI](openapi/cms-gov-marketplace-openapi.yml)
- [Naftiko Capability — Marketplace Plans](capabilities/marketplace-plans.yaml)

### CMS Open Data API (data.cms.gov)

Public catalog of CMS datasets — Medicare provider utilization, Open Payments, Compare datasets, Marketplace public-use files, and more — queryable via JSON/CSV and dataset-level data-api endpoints.

**Human URL:** [https://data.cms.gov/](https://data.cms.gov/)

- [DCAT Catalog](https://data.cms.gov/data.json)
- [OpenAPI](openapi/cms-gov-open-data-openapi.yml)
- [Naftiko Capability — Open Data Datasets](capabilities/open-data-datasets.yaml)

### CMS Provider Data Catalog API

Quality and compare datasets that powered the legacy Hospital Compare, Nursing Home Compare, Home Health, Hospice, LTCH, IRF, Dialysis, and Physician Compare sites via CKAN/DKAN-compatible endpoints.

**Human URL:** [https://data.cms.gov/provider-data/](https://data.cms.gov/provider-data/)

- [Documentation](https://data.cms.gov/provider-data/docs)
- [OpenAPI](openapi/cms-gov-provider-data-openapi.yml)
- [Naftiko Capability — Provider Data Catalog](capabilities/provider-data-catalog.yaml)

### CMS Quality Payment Program API

MIPS and Advanced APM submission and scoring under MACRA. Used by Qualified Registries, EHR vendors, and QCDRs.

**Human URL:** [https://qpp.cms.gov/about/resource-library](https://qpp.cms.gov/about/resource-library)

- [Source Code — qpp-measures-data](https://github.com/CMSgov/qpp-measures-data)
- [OpenAPI](openapi/cms-gov-qpp-openapi.yml)
- [Naftiko Capability — Quality Payment Program](capabilities/quality-payment-program.yaml)

### CMS Medicare Coverage Database API

National Coverage Determinations (NCDs), Local Coverage Determinations (LCDs), articles, and MEDCAC records for Medicare coverage policy.

**Human URL:** [https://www.cms.gov/medicare-coverage-database/](https://www.cms.gov/medicare-coverage-database/)

- [OpenAPI](openapi/cms-gov-mcd-openapi.yml)
- [Naftiko Capability — Medicare Coverage Database](capabilities/medicare-coverage-database.yaml)

## Common

- [Portal — CMS Homepage](https://www.cms.gov/)
- [Portal — CMS Developer Hub](https://developer.cms.gov/)
- [SourceCode — CMSgov GitHub Org](https://github.com/CMSgov)
- [Forum — Blue Button Google Group](https://groups.google.com/g/developer-group-for-cms-blue-button-api)
- [Forum — BCDA Google Group](https://groups.google.com/g/cms-bcda-api)
- [Forum — AB2D Google Group](https://groups.google.com/g/cms-ab2d-api)
- [Sandbox — Blue Button](https://bluebutton.cms.gov/developers/#try-the-api)
- [Sandbox — BCDA](https://sandbox.bcda.cms.gov/)
- [Sandbox — AB2D](https://sandbox.ab2d.cms.gov/)
- [Sandbox — DPC](https://sandbox.dpc.cms.gov/)
- [Documentation — CARIN Blue Button FHIR IG](https://hl7.org/fhir/us/carin-bb/)
- [Documentation — HL7 FHIR Bulk Data Access IG](https://hl7.org/fhir/uv/bulkdata/)
- [Privacy Policy](https://www.cms.gov/about-cms/web-policies-important-links/privacy-policy)

## Artifacts

- OpenAPI specs in `openapi/`
- JSON Schema resources in `json-schema/`
- JSON-LD context in `json-ld/`
- Examples in `examples/`
- Naftiko capabilities in `capabilities/`
- Spectral ruleset in `rules/cms-gov-rules.yml`
- Vocabulary in `vocabulary/cms-gov-vocabulary.yml`
- Rate-limit policies in `rate-limits/cms-gov-rate-limits.yml`

## Maintainers

- **Centers for Medicare & Medicaid Services** — [https://www.cms.gov/](https://www.cms.gov/) — `CMS_Feedback@cms.hhs.gov`
