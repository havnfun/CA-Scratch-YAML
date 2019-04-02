<!--- Text entered into this file will appear at the top of the profiles page before the Formal Views of the profile content. -->

This profile was generated from [HL7 StructureDefinition](https://www.hl7.org/fhir/medication.profile.json) on 2019-03-28 and constrained during a review of US Core against Canadian sources.  RxNorm is not used in Canada and the list of medicinal products available differs from the US, therefore [PrescribeIT Medication Profile](https://specs.prescribeit.ca/R2.0/erx/profile-medication.html) was used as a basis for this profile - with some significant differences due to structural differences between versions of FHIR.

Key differences from [USCoreR4 Medication](https://build.fhir.org/ig/HL7/US-Core-R4/StructureDefinition-us-core-medication.html):
- RxNorm is not used in Canada, replaced with a Canadian list of MedicationForm

Key differences from PrescribeIT Medication Profile](https://specs.prescribeit.ca/R2.0/erx/profile-medication.html):
- Medication.id left with FHIR defaults
- Medication.product element has been deleted from FHIR, used Medication.form, Medication.ingredient, Medication.amount instead of equiv. elements in Medication.product
- [ext-medication-strength-description](https://specs.prescribeit.ca/R2.0/erx/extension-ext-medication-strength-description.html) removed because it appears to be semantically equiv. to Medication.amount **<< might not meet requirement**

**Note:**
- mustSupport reflects PrescribeIT **<< many more requirements here than in USCoreR4 ... must these all be supported**
- Medication.ingredient.item[x] is currently restricted in a manner consistent with the PrescribeIT Medication profile.  **<< Is this preferable to providing references to other Medication (and potentially Substance) resources?**
- [ON DHDR](https://simplifier.net/ontariodigitalhealth/medication) and [HL7 v3 AdministerableMedicine](AdministerableMedicine) appear to approach similar things differently than below.

**[ToDo]:**

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

{% include link-list.md %}