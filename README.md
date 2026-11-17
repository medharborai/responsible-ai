# Responsible AI at MedHarbor

How the AI in [MedHarbor](https://medharborai.com) is designed: what it does, what it does not do and the rules we follow.

> **Please note:** MedHarbor is in development. The product does not exist yet and does not process any health data today. This page describes how we are designing it and the commitments we are making for the product we are building. We will update it as the prototype and the pilot progress.

## What the AI does

MedHarbor will help people turn their scattered medical documents into one clear patient card that any doctor can read in their own language.

- **Reads documents.** Photos, scans and PDFs in any language, including handwritten notes.
- **Recognises the document type.** Discharge letter, lab report, prescription, vaccination record.
- **Picks out the key facts.** Diagnoses, medication, allergies, test results, procedures and vaccinations, with international codes (ICD-10, ATC, LOINC).
- **Shows its sources.** Every fact links back to its page in the original document, and the card shows how sure the AI is about each fact.
- **Writes the card in the doctor's language.** The most important facts come first: allergies, current medication, chronic conditions. The full history follows.

Planned later: medicines abroad (the active ingredient and local equivalents of each medicine) and an appointment helper with translation during the visit.

## What the AI does not do

- It does **not** diagnose.
- It does **not** interpret test results.
- It does **not** recommend or change treatment, or give medical advice.
- It is **not** trained on users' records. Our AI providers will be barred by contract from training on them.
- It does **not** sell or share health data, show ads, promote medicines or take commission from pharmacies or drug makers.

MedHarbor organises, translates and shares records. It is designed not to be a medical device.

## Who decides

- **The patient** checks the card before sharing it. Allergies and medication always need the patient's confirmation.
- **The patient** decides who sees the card and for how long. Each shared card expires when the patient decides, and access can be revoked at any time.
- **The doctor** makes every medical decision. The card is a clear summary with links to the originals, not a diagnosis.

Our principle: a summary without a source is worse than no summary.

## Data and consent

These are our commitments for the product we are building:

- **Data stays in the EU.** Documents, extracted data and cards will be stored and processed only in EU data centres.
- **Always encrypted.** Data will be encrypted both when stored and when sent.
- **Explicit consent.** We will only process health data with the user's explicit consent, which can be withdrawn at any time.
- **Minimal access.** Only people who need access will get it, and every access is logged. Where possible, names are removed before AI processing.
- **Delete everything in one tap.** Deleting an account removes all documents, data and cards.
- **Independent checks.** A data protection impact assessment and an independent security test before any public launch.

## Rules we are building for

| Rule | What it means for MedHarbor |
| --- | --- |
| EU MDR (medical devices) | MedHarbor only organises, translates and shares records. It does not diagnose, interpret results or give treatment advice. A formal review will take place before the pilot. |
| GDPR, Article 9 | Explicit consent, impact assessment, only the data we need, EU hosting. |
| EU AI Act | AI-generated content is clearly labelled, and model versions are logged. |
| EHDS and HL7 FHIR | Cards use the International Patient Summary format so they can work with other health systems later. |

## How we will test it

In the pilot, the accuracy of the cards will be checked by a doctor. Our target is at least 90 % of facts correct, with no errors in allergies or medication.

## Contact

Questions or suggestions about this page: open an issue in this repository or email [info@medharborai.com](mailto:info@medharborai.com).

Security issues: see our [security policy](https://github.com/medharborai/.github/blob/main/SECURITY.md).

Website: [medharborai.com](https://medharborai.com)

## Licence

This document is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You may share and adapt it, including for commercial purposes, as long as you credit MedHarbor and link to this repository.

The MedHarbor name and logo are not covered by this licence.
