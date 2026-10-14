# Clinical content and ECG provenance — development register

## Status
Prototype only. No independent clinical review, no validated scoring, and no real ECG image integrated yet. All presented patient details, troponin values and ECG descriptions are fictional.

## Intended ECG dataset
PTB-XL v1.0.3, PhysioNet, https://physionet.org/content/ptb-xl/1.0.3/ ; DOI 10.13026/kfzx-aw45 ; CC BY 4.0. Dataset contains 21,799 clinical 12-lead ECG records. A source recording must be selected and inspected for morphology, signal quality, leads, metadata and scenario compatibility **before** display. The dataset does not establish that the ECG belongs to this fictional ED patient.

## ECG ingestion acceptance checklist
- Source dataset and version, original record identifier, direct attribution and licence retained.
- Source waveform decoded and displayed at correct voltage/time calibration with lead labels.
- Clinician verifies ECG findings match the simulated presentation.
- No claim that a composite patient is a real patient.
- If a second ECG is used, do not falsely represent two different patient recordings as serial ECGs from one person.
- Avoid unlicensed educational-site screenshots.
- Mobile display tested for legibility and zoom.

## Clinical reference
NICE CG95 https://www.nice.org.uk/guidance/cg95/chapter/recommendations ; NICE NG185 https://www.nice.org.uk/guidance/ng185

NICE CG95 recommends prompt ECG, serial ECG consideration when ACS is uncertain, monitoring and clinical context when interpreting high-sensitivity troponin. Troponin algorithms must be assay-specific. This prototype's current timing, scoring and outcomes are illustrative, not an implementation of a validated diagnostic algorithm.

## Planned scenario engine
Each action should record its time, prerequisites, turnaround time, result, cost to simulated clinical time, patient state effects and assessment tags. Explicit branching must distinguish deterioration, delayed escalation, reassessment and disposition. Clinical review and safety testing are required before broader educational deployment.
