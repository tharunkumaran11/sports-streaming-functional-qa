# Sports Streaming Functional Testing and Media QA

Independent AI-assisted portfolio project. Test execution is recorded complete following the user’s manual confirmation on 24 November 2026. This is not an Amazon production audit or release approval.

| Metric | Current result |
| --- | ---: |
| Planned checks | 40 |
| PASS | 40 |
| FAIL in the original 40 checks | 0 |
| BLOCKED | 0 |
| PENDING | 0 |
| Recorded execution coverage | 100% |
| Codex-observed passes | 20 |
| User-reported manual passes | 20 |
| Supplemental accessibility defect | 1 open |

## Evidence and attribution

Codex freshly retested loading, play/pause, forward/backward seeking and sampled visual quality on five original ICC videos. Those 20 passes have saved browser observations and screenshots. All five original assets played; no replacements were required.

The remaining 20 checks were initially blocked or inconclusive. The user subsequently stated “all fine” and confirmed that all four checks passed for all five videos, including actual full-screen expansion, audible mute/volume, audio clarity/synchronization and testing on a real phone. These are now recorded as **user-reported manual PASS**, supported by the chat attestation in [evidence/manual_confirmation.json](evidence/manual_confirmation.json).

**The manual results were not independently observed by Codex.** Phone model, computer/phone browser versions, exact manual execution date and supporting screenshots/recordings were not supplied. Manual execution date cells therefore remain blank; the confirmation date is recorded separately. Do not describe this as 40 independently evidenced automated passes. The original browser observations and earlier limitations remain in the evidence history.

DEF-01 remains open: the seek slider’s accessible time label stays zero while the displayed time advances. The user’s confirmation of the original four blocked checks does not establish that this separate accessibility issue was fixed. A QA project can finish execution while reporting an open defect.

## Deliverables

- [Functional_Test_Results.xlsx](Functional_Test_Results.xlsx): 40 results, formulas and evidence attribution, with original Assets and Test cases retained.
- [Defect_Report.xlsx](Defect_Report.xlsx) and [DEFECTS.md](DEFECTS.md): open defect and follow-up history.
- [Execution_Results.csv](Execution_Results.csv) and [metrics.json](metrics.json): matching readable results and metrics.
- [Testing_SOP.md](Testing_SOP.md) and [Testing_SOP.docx](Testing_SOP.docx): matching procedures. Word text/structure was checked; visual pagination could not be verified because no Word/LibreOffice renderer was available.
- [evidence/INDEX.md](evidence/INDEX.md): saved browser evidence and the subsequent manual attestation.
- [PROVENANCE.md](PROVENANCE.md): AI/user attribution and original-package history.
- [VERIFICATION.md](VERIFICATION.md) and [SHA256SUMS.txt](SHA256SUMS.txt): package checks and file hashes.

## Reproduction and GitHub use

Open the five URLs in the Assets worksheet and follow the SOP. Record observed results with date, device/browser and evidence. PASS requires the expected result; FAIL records a reproducible discrepancy. Keep unsupported checks BLOCKED and unattempted checks PENDING. If more detailed manual evidence becomes available, append it to the existing record rather than replacing the original AI observations.

The summary counts status cells in Execution. Coverage = (PASS + FAIL) / planned; pass rate = PASS / (PASS + FAIL). Current metrics include the user’s 20 reported passes. DEF-01 is supplemental to the original eight cases per asset and is excluded from the 40-case denominator.

Published repository: https://github.com/tharunkumaran11/sports-streaming-functional-qa. The downloadable ZIP preserves the same relative paths. Keep the AI-assisted provenance and manual-attestation limitations visible. Third-party ICC screenshots are retained as QA evidence; no ownership or general content license is asserted over third-party material, and source videos/audio are not redistributed.
