# Evidence index

## Subsequent manual confirmation

The user confirmed all four previously blocked checks passed on each of the five videos, including a real phone. See [manual_confirmation.json](manual_confirmation.json) for the 20 user-reported PASS records, missing device/browser details and preserved prior observations. No new user captures were supplied. The sections below describe the earlier AI-only evidence and its limitations; statements that cases are blocked are historical, not the current execution status.

## AI retest evidence history

Fresh AI-assisted browser retest on 24 November 2026. Raw observations: [observations.json](retest/observations.json). Filter by asset and label. Timestamps are UTC; add 05:30 for IST. Historical screenshots remain inside the unmodified original ZIP in provenance/.

Each FT02/FT03 result requires the raw log sequence; a single still image alone does not prove time stability or seeking. FT05, FT07 and FT08 retain their original audible/phone criteria and are blocked despite partial observations. Full-screen images do not establish expansion.

| Asset | Page | Beginning | Middle | Late | Responsive | Volume |
| --- | --- | --- | --- | --- | --- | --- |
| C01 | [Kohli delivers in his final T20I | POTM highlights | SA v IND | T20WC 2024 Final](https://www.icc-cricket.com/tournaments/t20cricketworldcup/videos/kohli-delivers-in-his-final-t20i-potm-highlights-sa-v-ind-t20wc-2024-final) | [Beginning](retest/C01_pause_stable.png) | [Middle](retest/C01_visual_middle_ready.png) | [Late](retest/C01_visual_end.png) | [390 × 844](retest/C01_mobile_pause.png) | [Slider](retest/C01_volume_mid.png) |
| C02 | [India win their second T20 World Cup title | Extended Highlights | SA v IND | T20WC 2024 Final](https://www.icc-cricket.com/tournaments/t20cricketworldcup/videos/india-win-their-second-t20-world-cup-title-extended-highlights-sa-v-ind-t20wc-2024-final) | [Beginning](retest/C02_pause_stable.png) | [Middle](retest/C02_visual_middle_ready.png) | [Late](retest/C02_visual_end.png) | [390 × 844](retest/C02_mobile_pause.png) | [Slider](retest/C02_volume_mid.png) |
| C03 | [India script stunning title win | Match Highlights | SA v IND | T20WC 2024 Final](https://www.icc-cricket.com/tournaments/t20cricketworldcup/videos/india-script-stunning-title-win-match-highlights-sa-v-ind-t20wc-2024-final) | [Beginning](retest/C03_pause_stable.png) | [Middle](retest/C03_visual_middle_ready.png) | [Late](retest/C03_visual_end.png) | [390 × 844](retest/C03_mobile_pause.png) | [Slider](retest/C03_volume_mid.png) |
| C10 | [Quinton Kock - Wicket - South Africa vs India](https://www.icc-cricket.com/tournaments/t20cricketworldcup/videos/quinton-kock-wicket-south-africa-vs-india) | [Beginning](retest/C10_pause_stable.png) | [Middle](retest/C10_visual_middle_ready.png) | [Late](retest/C10_visual_end.png) | [390 × 844](retest/C10_mobile_pause.png) | [Slider](retest/C10_volume_mid.png) |
| C05 | [Unbelievable catch from SKY | SA v IND | T20WC 2024 Final](https://www.icc-cricket.com/tournaments/t20cricketworldcup/videos/unbelievable-catch-from-sky-sa-v-ind-t20wc-2024-final) | [Beginning](retest/C05_pause_stable.png) | [Middle](retest/C05_visual_middle_ready.png) | [Late](retest/C05_visual_end.png) | [390 × 844](retest/C05_mobile_pause.png) | [Slider](retest/C05_volume_mid.png) |

## Playback sample positions

| Asset | Duration s | Beginning s | Middle s | Late s |
| --- | ---: | ---: | ---: | ---: |
| C01 | 205.400 | 18.733 | 106.066 | 200.400 |
| C02 | 571.920 | 20.411 | 285.753 | 516.386 |
| C03 | 329.080 | 0.463 | 169.567 | 306.357 |
| C10 | 32.194 | 10.060 | 16.085 | 27.194 |
| C05 | 29.200 | 4.304 | 14.589 | 24.200 |

## Observation labels

- loading/loading_recheck: decoded current media state. C01 uses loading_recheck screenshot.
- pause and pause_stable: same position across a multi-second interval.
- resume, seek_forward and seek_back: actual playback positions and readiness after input.
- mute and unmute: observed state only; volume_ui includes the actual slider label.
- visual_middle_ready and visual_end: final reviewed samples. Intermediate *_seek and visual_middle records may show buffering and are not used alone as quality proof.
- mobile_play/mobile_seek/mobile_pause: desktop responsive interactions, not a real phone.
- fullscreen/exit_fullscreen: button transition observations; inconclusive expansion.

No audio evidence file exists because no listening or audio recording was performed. No screenshot is treated as proof of sound.
