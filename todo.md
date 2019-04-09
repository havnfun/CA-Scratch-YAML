##ToDo List

**profile-allergyintolerance:**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs
- review against PrescribeIT and DHDR **<< outstanding**

[] review and update terminology bindings

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-condition**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3

[x] review structure against existing CAD FHIR specs

[x] review and update terminology bindings
- [US Core Condition Category Codes](https://build.fhir.org/ig/HL7/US-Core-R4/ValueSet-us-core-condition-category.html) extends the default list used here with additional value health-concern **<< is this needed?**
- The [HL7 ConditionCode ValueSet](http://hl7.org/fhir/ValueSet/condition-code) on the base FHIR Condition resource appears to provide a shorter list of common Dx **<< which is preferable?**

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-device**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3
- [HL7v3 ManufacturedClinicalDevice](https://infocentral.infoway-inforoute.ca/extra/ca/mr0206-html/html/message.html?COCT_MT141007CA)

[x] review structure against existing CAD FHIR specs
- No Canadian profiles on FHIR Device resource were identified on quick review of the [Canadian FHIR Registry](https://simplifier.net/organization/canadianfhirregistry)

[x] review and update terminology bindings
- USCoreR4 Device.type is bound to valueSet [device-kind](http://build.fhir.org/valueset-device-kind.html)
- base FHIR resource is bound to [device-type](http://build.fhir.org/valueset-device-type.html)
- the valueSets appear to be identical but the former is used less frequently (only on Device)
- used the binding in USCoreR4.

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-encounter**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs

[] review [US_Core_Encounter_Type](http://build.fhir.org/ig/HL7/US-Core-R4/ValueSet-us-core-encounter-type.html) valueSet against CAD equiv and update **Encounter.type** binding (if necessary)

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-immunization**

[X] review USCoreR4 profile and draft extensions and restrictions

[X] review structure against pan-CDN HL7 v3
- scanned only

[x] review structure against existing CAD FHIR specs
- Note that [ICON](https://simplifier.net/digitalhealthimmuniz/~resources?category=Profile&sortBy=RankScore_desc) has a number of different profiles, review was not exhaustive
  - Immunization.statusReason is not here assuming intent is the same as Immunization.explanation.reason in ICON spec

[x] review and update terminology bindings
- needs review / refinement

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-location**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3

[x] review structure against existing CAD FHIR specs

[x] review and update terminology bindings

[] PRN, LN identifier.system: **should the list of URIs be constrained using valueSets?**

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-medication**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against existing CAD FHIR specs
- Further review of requirements / use of PrescribeIT Medication.product
- Review requirements / use of ProscribeIT [ext-medication-code-representative](https://specs.prescribeit.ca/R2.0/erx/extension-ext-medication-code-representative.html)
- Review ON DHDR implementations?

[] review structure against pan-CDN HL7 v3
- Review CAD HL7 v3 implementations?

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-medicationrequest**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs
- review against PrescribeIT and DHDR **<< outstanding**

[] review and update terminology bindings

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-medicationstatement**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs
- review against PrescribeIT and DHDR **<< outstanding**

[] review and update terminology bindings

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-observation**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs

[] review and update terminology bindings
- update Observation.code binding to pCLOCD

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-organization**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3

[x] review structure against existing CAD FHIR specs

[x] review and update terminology bindings

[] PRN, LN identifier.system: **should the list of URIs be constrained using valueSets?**

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-patient:**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3

[x] review structure against existing CAD FHIR specs

[x] review and update terminology bindings

[] identifier:JHN.system: **should the list of URIs be constrained using a valueSet?**

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-practitioner**

[x] review USCoreR4 profile and draft extensions and restrictions

[x] review structure against pan-CDN HL7 v3

[x] review structure against existing CAD FHIR specs

[x] review and update terminology bindings

[] PRN, LN identifier.system: **should the list of URIs be constrained using valueSets?**

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile=practitionerrole**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs

[] review [PractitionerRole](http://build.fhir.org/valueset-practitioner-role.html) against CDN specs

[] review [PracticeSettingCodeValueSet](http://build.fhir.org/valueset-c80-practice-codes.html) against CDN specs

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

**profile-proceure**

[x] review USCoreR4 profile and draft extensions and restrictions

[] review structure against pan-CDN HL7 v3

[] review structure against existing CAD FHIR specs

[] review and update terminology bindings
- Procedure.code binding from USCoreR4 not carried forward due to inclusion of AMA CPT coding not typically used in Canada
- http://hl7.org/fhir/ValueSet/procedure-code valueset has been retained although it is broader than the list of [Professional Service Codes](https://infocentral.infoway-inforoute.ca/extra/ca/mr0206-html/html/vocabulary.html?type=vs&id=ActProfessionalServiceCode) which appears to be used in the Canadian HL7v3 specs.

[] add constraints (cross element) from USCoreR4

[] refine constraints (cross element) to CAD requirements ?

[] ?

{% include link-list.md %}
