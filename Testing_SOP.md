# Sports Streaming Functional QA SOP

Scope: five original ICC cricket clips, eight checks per clip. Record actual observed results. This is an independent AI-assisted portfolio exercise. Historical screenshots are not fresh execution evidence.

FT01  Video loading: Open page and start video. Expected: Rendered video frame appears.

FT02  Play and pause: Play, pause, wait, resume. Expected: Time stops on pause and advances on resume.

FT03  Seeking: Seek forward and backward. Expected: Playback resumes at both selected positions.

FT04  Full screen: Enter and exit full screen. Expected: Player changes mode and returns.

FT05  Mute and volume: Mute, unmute and adjust volume. Expected: Audible output changes as expected.

FT06  Visual quality: Inspect beginning, middle and end. Expected: No major visible distortion in samples.

FT07  Audio quality: Listen to commentary and compare action. Expected: Clear audio with no obvious sync issue.

FT08  Mobile compatibility: Open on phone and exercise controls. Expected: Player fits screen and controls work.

Record browser and device, date and time, observations and evidence. PASS requires the entire expected result. FAIL requires a reproducible discrepancy. Use BLOCKED for unsupported, partially verified or inconclusive acceptance checks. Use PENDING for checks not attempted. Retain evidence and history when retesting.

Record browser/device, date, observation and evidence. PASS only when the expected result is observed. FAIL only when a reproducible discrepancy is established; otherwise keep PENDING. Retest failures and record steps, severity and evidence in the defect report. Do not infer audio from screenshots or mobile compatibility from desktop views.

Retest evidence and current outcome

Current result recorded on 24 November 2026: 40 PASS, 0 FAIL, 0 BLOCKED and 0 PENDING. Twenty passes were observed by Codex during the browser retest. The user subsequently confirmed the other 20 checks passed, including a real phone. Coverage and evaluated pass rate are 100 percent on that combined basis. Manual device/browser details, exact execution dates and supporting captures were not supplied.

Fresh Chrome interactions established loading, pause stability with resumed playback, forward and backward seeking, and reviewed beginning, midpoint and late visual samples. Use evidence/INDEX.md and evidence/retest/observations.json to trace each result. UTC observation times convert to IST by adding 5 hours 30 minutes. Preserve original evidence in the provenance archive.

Manual acceptance checks and reproducibility

Full screen: open each asset in a regular browser, enter and exit full screen, and verify actual expansion and return. The automated captures only established a label change. Record any browser limitation and do not pass the check from the label alone.

Mute and volume: use speakers or headphones at a comfortable level. Verify audible mute and unmute, then low, medium and high volume. The retest established state and slider changes only. Record listening observations with timestamps.

Audio quality: listen at beginning, middle and late positions. Assess commentary clarity, obvious clipping, unexplained dropouts and alignment with visible action. A visible mute state or an audio track alone does not establish quality or synchronization.

Mobile: open all five URLs on an actual phone. Record model, OS, browser version, orientation and network. Exercise play, pause, seek, mute and full screen where supported. Verify fit and usable touch controls. The 390 by 844 desktop viewport evidence is partial responsive testing only.

Record issues and finalize metrics

DEF-01 records the stale seek slider accessibility label on all five assets. It is a supplemental DOM observation, outside the 40 original cases; screen reader behavior remains untested. OBS-01 records inconclusive full-screen expansion. Reproduce issues, record expected versus actual behavior, severity, steps and evidence, and distinguish product defects from test-environment restrictions.

Update Execution status, observations, date, executor and evidence after each retest. Coverage equals PASS plus FAIL divided by planned checks. Pass rate equals PASS divided by PASS plus FAIL. Keep blocked cases visible. Reconcile the workbooks, CSV, metrics and README before packaging; update file checksums after any edit. Preserve AI-assisted provenance and avoid claiming human testing that did not occur.

User confirmation and evidence limits

The four manual-check procedures above describe what the user confirmed passed on all five videos. The text about automated capture and listening limitations preserves the AI-only test history. Current user-reported results are in evidence/manual_confirmation.json. Codex did not independently observe the manual tests. Execution-date cells are blank for those results because the actual test date was not supplied. DEF-01 remains open. DOCX visual pagination was not verified; use Testing_SOP.md for reliable text review.
