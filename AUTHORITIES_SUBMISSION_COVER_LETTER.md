# Authorities Submission Cover Letter (Template)

> This template is not legal advice. Adjust to your jurisdiction, agency requirements, and counsel guidance.

**Date:** <YYYY-MM-DD>  
**From:** <YOUR_ORG_NAME / INVESTIGATOR NAME>  
**Role/Title:** <ROLE>  
**Organization:** <ORG>  
**Address:** <ADDRESS>  
**Phone/Email:** <CONTACT>  

**To:** <AGENCY / PROSECUTOR / COURT / REGULATOR>  
**Attn:** <RECIPIENT NAME/TITLE>  
**Reference:** <CASE NAME / FILE # / DOCKET # / INCIDENT #>  

## Subject
Submission of Digital Forensic Evidence Package — <CASE NAME / FILE #>

## 1) Purpose of Submission
This letter accompanies a digital forensic evidence package related to:
- **Case/Incident:** <CASE NAME>
- **Reference/File #:** <REFERENCE>
- **Scope summary:** <1–3 sentences summarizing what was analyzed and why>

The objective is to provide a verifiable, reproducible set of artifacts to support review and (where applicable) legal proceedings.

## 2) Legal Authority (Stage 1)
The undersigned affirms that evidence collection and analysis were conducted under the following authority:
- **Authority basis:** <WARRANT / CONSENT / ORGANIZATIONAL POLICY / OTHER>
- **Authority reference:** <WARRANT # / CONSENT FORM ID / POLICY ID>
- **Responsible custodian:** <NAME / TITLE>

## 3) Contents of the Evidence Package (Stage 2–3)
The package includes:
1. **Executive Forensic Report (PDF)** — high-level findings and conclusions  
2. **Technical Forensic Report (PDF)** — detailed methodology, tool outputs, limitations  
3. **Evidence Manifests** — per-evidence ID metadata including SHA-256 and MD5 hashes  
4. **Chain-of-Custody Log (JSONL)** — append-only record of evidence intake and processing events  
5. **Original Evidence Files** (as available and permitted)  
6. **Derived Artifacts** (e.g., extracted audio, metadata summaries), linked to evidence IDs and hashes  

**Package filename:** `evidence_package.zip`  
**Package hash (SHA-256):** <SHA256_OF_ZIP>  

## 4) Chain of Custody Summary (Stage 5)
Evidence handling was documented using:
- Unique evidence identifiers (EVID-…)
- Cryptographic hashing at intake (SHA-256, MD5)
- Append-only custody logging of case actions (creation, upload, analysis, report generation, export)

Transfers of custody should be recorded by the receiving authority according to their procedures. If physical media was used, indicate:
- Media type/serial: <USB/DRIVE SERIAL>
- Tamper seal IDs: <SEAL IDs>
- Transfer date/time/location: <DETAILS>

## 5) Verification Instructions (Stage 6)
To verify integrity:
1. Compute SHA-256 for `evidence_package.zip` and confirm it matches this letter and/or the included manifest.
2. Extract the ZIP.
3. For each evidence item:
   - confirm the SHA-256/MD5 in `manifest.json`
   - optionally recompute hashes of the corresponding files
4. Review custody log (`custody.log.jsonl`) for the chronological record.
5. Review reports (Executive/Technical). Each report page includes a footer listing sources (evidence IDs, tools, and methods).

## 6) Methodology & Limitations
The reports document the methodology aligned with a standard six-stage forensic lifecycle:
- Legal authority & preparation
- Evidence identification and preservation
- Acquisition/imaging (where applicable)
- Analysis using forensic tools
- Documentation and chain of custody
- Presentation and integrity verification

**Limitations/notes:** <E.g., platform constraints, missing source data, encryption, partial capture, etc.>

## 7) Declaration
I, <NAME>, attest that to the best of my knowledge:
- The submitted package is a faithful representation of the collected and analyzed digital artifacts within scope.
- Hashes and custody logs were generated to preserve integrity and reproducibility.
- Conclusions in the reports are based on documented artifacts and stated methods.

**Signature:** __________________________  
**Name:** <NAME>  
**Title:** <TITLE>  
**Date:** <YYYY-MM-DD>  

## 8) Attachments
- `evidence_package.zip`
- Any required authority documentation (warrant/consent/policy extracts), as permitted
- Any supplemental exhibit index, if required by the receiving authority
