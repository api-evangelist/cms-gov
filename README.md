# CMS — Centers for Medicare & Medicaid Services (cms-gov)

The Centers for Medicare & Medicaid Services (CMS) is the U.S. federal agency within the Department of Health and Human Services that administers Medicare, Medicaid, the Children's Health Insurance Program (CHIP), the Health Insurance Marketplace, and the broader CMS open-data program. CMS operates one of the largest collections of HL7 FHIR APIs in the U.S. federal government — Blue Button 2.0, BCDA, AB2D, DPC, and the upstream BFD server — alongside the Marketplace API, the data.cms.gov open-data catalog, the Provider Data Catalog, the Quality Payment Program API, and the Medicare Coverage Database.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Healthcare
- Medicare
- Medicaid
- FHIR
- Bulk Data
- Open Data
- Government
- Federal
- Claims
- Insurance
- ACA
- Marketplace
- Quality

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### CMS Blue Button 2.0 API

Blue Button 2.0 is a developer-friendly, OAuth 2.0-enabled, HL7 FHIR R4 standard data API that delivers Medicare Part A, B, and D claims data for 60+ million Medicare beneficiaries to applications, services, and research programs. Includes Patient, Coverage, and ExplanationOfBenefit resources for the beneficiary's consented data.

- **Human URL:** [https://bluebutton.cms.gov/developers/](https://bluebutton.cms.gov/developers/)
- **Base URL:** `https://api.bluebutton.cms.gov/v2/fhir`

#### Tags

- Healthcare
- Medicare
- FHIR
- Claims
- Beneficiary
- Government

#### Properties

- [Documentation](https://bluebutton.cms.gov/developers/)
- [Console](https://bluebutton.cms.gov/api/v2/explorer/)
- [OpenAPI](openapi/cms-gov-blue-button-2-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-blue-button-2.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-blue-button-2.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/cms-gov-explanation-of-benefit-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/cms-gov-patient-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/cms-gov-coverage-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/cms-gov-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### CMS Beneficiary Claims Data API (BCDA)

BCDA enables Medicare Shared Savings Program Accountable Care Organizations (ACOs) to retrieve bulk Medicare Parts A, B, and D claims data for their assigned and assignable beneficiaries via the HL7 FHIR Bulk Data Access (Flat FHIR) specification. Uses asynchronous $export endpoints returning NDJSON resources for Patient, Coverage, and ExplanationOfBenefit.

- **Human URL:** [https://bcda.cms.gov/](https://bcda.cms.gov/)
- **Base URL:** `https://api.bcda.cms.gov/api/v2`

#### Tags

- Healthcare
- Medicare
- FHIR
- Bulk Data
- ACO
- Claims
- Government

#### Properties

- [Documentation](https://bcda.cms.gov/)
- [Documentation](https://bcda.cms.gov/guide.html)
- [Sandbox](https://sandbox.bcda.cms.gov/)
- [OpenAPI](openapi/cms-gov-bcda-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-bcda.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-bcda.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS AB2D API

AB2D (Claim and Claim Line Feed) delivers Medicare Parts A, B, and D claims data to Part D prescription drug plan sponsors via the HL7 FHIR Bulk Data Access specification. Supports asynchronous $export of ExplanationOfBenefit resources as NDJSON for all enrolled Medicare beneficiaries since 2020.

- **Human URL:** [https://ab2d.cms.gov/](https://ab2d.cms.gov/)
- **Base URL:** `https://api.ab2d.cms.gov/api/v2`

#### Tags

- Healthcare
- Medicare
- FHIR
- Bulk Data
- Part D
- Claims
- Government

#### Properties

- [Documentation](https://ab2d.cms.gov/)
- [Documentation](https://ab2d.cms.gov/getting-started/)
- [Console](https://sandbox.ab2d.cms.gov/swagger-ui/)
- [OpenAPI](openapi/cms-gov-ab2d-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-ab2d.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-ab2d.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Data at the Point of Care API (DPC)

Data at the Point of Care fills gaps in patient history by delivering Medicare claims data via HL7 FHIR Bulk Data Access to fee-for-service providers at the point of care. Providers register Practitioner, Organization, Group, and Patient roster resources, then asynchronously $export ExplanationOfBenefit, Coverage, and Patient resources.

- **Human URL:** [https://dpc.cms.gov/](https://dpc.cms.gov/)
- **Base URL:** `https://sandbox.dpc.cms.gov/api/v1`

#### Tags

- Healthcare
- Medicare
- FHIR
- Bulk Data
- Provider
- Government

#### Properties

- [Documentation](https://dpc.cms.gov/)
- [Documentation](https://dpc.cms.gov/docs)
- [OpenAPI](openapi/cms-gov-dpc-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-dpc.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-dpc.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Beneficiary FHIR Data Server (BFD)

The Beneficiary FHIR Data (BFD) Server is the upstream HL7 FHIR R4 service that powers Blue Button 2.0, BCDA, AB2D, and DPC. BFD ingests claims from the CMS Chronic Conditions Warehouse (CCW) and exposes Patient, Coverage, and ExplanationOfBenefit resources with both synchronous and bulk asynchronous access. Internal/peering access only; clients use the downstream Blue Button, BCDA, AB2D, or DPC APIs.

- **Human URL:** [https://bfd.cms.gov/](https://bfd.cms.gov/)

#### Tags

- Healthcare
- Medicare
- FHIR
- Claims
- Beneficiary
- Government

#### Properties

- [Documentation](https://bfd.cms.gov/)
- [Source Code](https://github.com/CMSgov/beneficiary-fhir-data)
- [OpenAPI](openapi/cms-gov-bfd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-bfd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-bfd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Marketplace API

The Marketplace API exposes Qualified Health Plan (QHP) and Stand-alone Dental Plan (SADP) data from healthcare.gov including plan finder, plan compare, plan rates, plan benefits, plan crosswalks, and issuer details. Powers consumer plan-shopping experiences across HealthCare.gov and partner brokers.

- **Human URL:** [https://developer.cms.gov/marketplace-api/](https://developer.cms.gov/marketplace-api/)
- **Base URL:** `https://marketplace.api.healthcare.gov/api/v1`

#### Tags

- Healthcare
- Marketplace
- Insurance
- ACA
- Plans
- Government

#### Properties

- [Documentation](https://developer.cms.gov/marketplace-api/)
- [Documentation](https://www.cms.gov/marketplace/resources/data/public-use-files)
- [OpenAPI](openapi/cms-gov-marketplace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-marketplace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-marketplace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Open Data API (data.cms.gov)

The CMS Open Data API exposes the full catalog of public CMS datasets — Medicare provider utilization and payment files, Medicare Advantage and Part D enrollment, Hospital Compare, Nursing Home Compare, Physician Compare, Open Payments (Sunshine Act), Marketplace public-use files, and the Provider Data Catalog. Datasets are queryable via filtered JSON/CSV downloads and dataset-level data-api endpoints.

- **Human URL:** [https://data.cms.gov/](https://data.cms.gov/)
- **Base URL:** `https://data.cms.gov/data-api/v1`

#### Tags

- Healthcare
- Open Data
- Datasets
- Socrata
- Government

#### Properties

- [Portal](https://data.cms.gov/)
- [Documentation](https://data.cms.gov/provider-data/)
- [Schema](https://data.cms.gov/data.json)
- [OpenAPI](openapi/cms-gov-open-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-open-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-open-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Provider Data Catalog API

The Provider Data Catalog API surfaces the quality and compare datasets that powered the legacy Hospital Compare, Nursing Home Compare, Home Health Compare, Hospice Compare, Long-Term Care Hospital Compare, Inpatient Rehabilitation Facility Compare, Dialysis Facility Compare, and Physician Compare sites via CKAN DKAN-compatible dataset and resource endpoints.

- **Human URL:** [https://data.cms.gov/provider-data/](https://data.cms.gov/provider-data/)
- **Base URL:** `https://data.cms.gov/provider-data/api/1`

#### Tags

- Healthcare
- Quality
- Provider
- Hospitals
- Compare
- Government

#### Properties

- [Portal](https://data.cms.gov/provider-data/)
- [Documentation](https://data.cms.gov/provider-data/docs)
- [OpenAPI](openapi/cms-gov-provider-data-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-provider-data.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-provider-data.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Quality Payment Program API

The Quality Payment Program (QPP) API supports the Merit-based Incentive Payment System (MIPS) and Advanced Alternative Payment Models (APMs) under MACRA. Exposes measures, benchmarks, scoring, and submission endpoints used by Qualified Registries, EHR vendors, and QCDRs to submit clinician performance data and retrieve scoring metadata.

- **Human URL:** [https://qpp.cms.gov/about/resource-library](https://qpp.cms.gov/about/resource-library)
- **Base URL:** `https://qpp.cms.gov/api`

#### Tags

- Healthcare
- Quality
- MIPS
- MACRA
- Provider
- Government

#### Properties

- [Documentation](https://qpp.cms.gov/about/resource-library)
- [Source Code](https://github.com/CMSgov/qpp-measures-data)
- [OpenAPI](openapi/cms-gov-qpp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-qpp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-qpp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CMS Medicare Coverage Database API

The Medicare Coverage Database (MCD) exposes National Coverage Determinations (NCDs), Local Coverage Determinations (LCDs), Local Coverage Articles, Proposed Decisions, National Coverage Analyses, and Medicare Evidence Development & Coverage Advisory Committee (MEDCAC) records. Powers coverage policy lookups by HCPCS code, ICD-10, contractor jurisdiction, and state.

- **Human URL:** [https://www.cms.gov/medicare-coverage-database/](https://www.cms.gov/medicare-coverage-database/)

#### Tags

- Healthcare
- Medicare
- Coverage
- Policy
- LCD
- NCD
- Government

#### Properties

- [Portal](https://www.cms.gov/medicare-coverage-database/)
- [Documentation](https://www.cms.gov/medicare-coverage-database/reports/reports.aspx)
- [OpenAPI](openapi/cms-gov-mcd-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cms-gov-mcd.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cms-gov-mcd.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://www.cms.gov/)
- [Portal](https://developer.cms.gov/)
- [Source Code](https://github.com/CMSgov)
- [Support](https://github.com/CMSgov/bluebutton-developer-help)
- [Forum](https://groups.google.com/g/developer-group-for-cms-blue-button-api)
- [Forum](https://groups.google.com/g/cms-bcda-api)
- [Forum](https://groups.google.com/g/cms-ab2d-api)
- [Support](https://dpc.cms.gov/contact)
- [Sandbox](https://bluebutton.cms.gov/developers/#try-the-api)
- [Sandbox](https://sandbox.bcda.cms.gov/)
- [Sandbox](https://sandbox.ab2d.cms.gov/)
- [Sandbox](https://sandbox.dpc.cms.gov/)
- [Authentication](https://bluebutton.cms.gov/developers/#authorization)
- [Authentication](https://bcda.cms.gov/guide.html#authentication)
- [Support](https://www.cms.gov/about-cms/contact-current/contact-us)
- [Blog](https://www.cms.gov/newsroom)
- [Privacy](https://www.cms.gov/about-cms/web-policies-important-links/privacy-policy)
- [Documentation](https://www.cms.gov/cclio/regulations-and-guidance)
- [Documentation](https://confluence.hl7.org/display/FHIR/Argonaut+Implementation+Guide+Home+Page)
- [Documentation](https://hl7.org/fhir/us/carin-bb/)
- [Documentation](https://hl7.org/fhir/uv/bulkdata/)
- [About](https://www.cms.gov/about-cms)
- [Feeds](https://www.cms.gov/about-cms/contact-current/cms-rss-feeds)

## Maintainers

**FN:** Centers for Medicare & Medicaid Services
**Email:** CMS_Feedback@cms.hhs.gov
**URL:** https://www.cms.gov/
