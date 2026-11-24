# Defect and observation report

Current follow-up on 24 November 2026: the user reports all 20 previously blocked cases passed, including a real-phone test. These are recorded as user-reported manual PASS. No device/browser details or new captures were supplied. DEF-01 remains open. The OBS/LIM sections below preserve the earlier AI-only test limitations and have been superseded for execution status by that user attestation; they remain limits of independent evidence.

## DEF-01 Seek slider accessible time stays zero

Status: Open. Severity: Low. Priority: P3. Type: Supplemental accessibility DOM defect. Observed on all five assets in Chrome desktop on 24 November 2026.

1. Open any URL in the Assets worksheet and allow playback to advance.
2. Pause or seek to a nonzero time.
3. Compare the displayed playback time with the seek slider’s accessible label in the DOM.

Expected: the slider exposes a meaningful current playback position and duration to accessibility APIs.

Actual: the seek slider label remains `00:00:00/00:00:00`, even when the displayed time is nonzero. For example, the C05 volume_ui snapshot has visible time `00:00:14 / 00:00:29` and slider label `00:00:00/00:00:00`; captured attributes also show no aria-valuenow. The C01, C02, C03 and C10 volume_ui snapshots reproduce the stale label with their respective nonzero times.

Evidence: evidence/retest/observations.json (filter label=volume_ui); evidence/retest/final_browser_state.txt. See the corresponding *_volume_mid.png for visible page context. The DOM issue is observed; actual screen reader impact was not tested. Do not claim WCAG compliance testing from this finding. Functional seeking still works, so the original FT03 acceptance criterion passes. This supplemental issue is outside the original 40 checks.

Suggested remediation: update the slider’s accessible value and duration as playback and seeking change. Retest with keyboard and screen reader on supported browsers; those checks are follow-up work, not completed tests.

## OBS-01 Full screen cannot be conclusively verified

Across the five assets, clicking Full Screen changes the button to Exit Full Screen. Captured screenshots remain embedded in the page. C01 and C02 read-only DOM observations reported fullscreen=false, and a native C02 click reproduced the same capture outcome. Expected screen expansion is not established. The source of the discrepancy may be the site, browser restrictions, or the capture interface. No root cause is assigned. FT04 is BLOCKED for all five assets, not a confirmed product FAIL.

Evidence: *_fullscreen.png, C02_fullscreen_native.png and the C01 fullscreen_dom log record. Recheck visually in a regular browser outside the capture interface before filing a production bug.

## LIM-01 Audible verification unavailable

Mute/unmute toggles and volume slider response were exercised. No listening or captured-audio analysis was performed. Audible mute/volume effects (FT05) and commentary clarity/synchronization (FT07) remain BLOCKED. A browser unmute state does not prove audible output.

## LIM-02 Physical mobile verification unavailable

All five players fit a 390 × 844 desktop viewport in the reviewed captures, with play/pause and backward-seek responses logged. This is partial responsive evidence. Physical phone, touch, iOS/Android browser behavior and orientation are unverified. FT08 remains BLOCKED against its original phone criterion.
