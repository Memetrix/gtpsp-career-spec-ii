# Gran Turismo PSP Career — public beta 0.27.2-beta.1

[Watch the public beta trailer](https://www.youtube.com/watch?v=EhzWIxJF08s).

This is the first public beta. It adds a GT4-style career to Gran Turismo PSP without replacing the original game modes. The beta includes a new cover, PSP menu icon and background.

## In this release

- **Career:** nine halls; 161 competitions adapted from GT4 Spec II 1.10 (credited in NOTICE) and two Lost Circuits events. Forty-two continuation cards keep longer series together, for 205 career cards and 763 rounds. Two additional Hidden Course Test cards are experimental and do not count toward completion.
- **Progression:** car restrictions, PSP Driving Challenge licence gates, credits, trophies and prize cars. Career progress uses a separate save slot. On first launch it can copy garage and credits from a stock PSP profile without overwriting that profile. The garage marks cars that fit an event.
- **Championships:** long seasons span six-round pages while retaining the same opponents and a single 10/8/6/4 points table. The championship reward is paid only after the final round. World Circuit Tour retains separate stage wins. Normal grids have four cars; Special Conditions are duels.
- **Tuning:** a shop for engine parts, tyres and suspension kits, with persistent ownership and fitted configuration. Ten engine categories use native car parameters: turbo, NA tune, exhaust, ECU, intercooler, port polish, weight reduction, engine balance, displacement and supercharger. Adjustable suspension and applicable brake controls are included. A Delta Integrale measured 7.596 s stock and 4.261 s fully upgraded from 0–100 km/h on the test oval. The purchase journal holds at most 192 tuned-car configurations.
- **Endurance:** 18 events have their full catalog distances or durations. Timed events accumulate distance across sessions; the same rivals and car settings continue, with a rolling start from the prior recorded positions. The 24-hour races use 72 twenty-minute sessions. Intermediate saves and final rewards are handled by the career.
- **Lost tracks:** Hong Kong, Rome Circuit, Complex String and Smokey Mountain previously crashed real PSP hardware; all four have since completed races on PSP Go. Tahiti Dirt has also passed a PSP Go hardware test. The two Lost Circuits events make these tracks part of the career.

## Known beta limits

- A complete accumulated 24-hour run has not yet been accepted. Lap-based endurance scoring and some race-result edge cases still need validation.
- On a resumed segment, the game's best-lap display can count the first partial lap as a short lap. Cumulative distance excludes that partial lap. The live position guide is an estimate; the confirmed result uses recorded race position.
- Complex String and Smokey Mountain still have visible texture and visibility defects. Hidden Course Test cards are diagnostic events and may fail.
- Opponent tuning and pace balance across all classes, and the remaining GT4 tuning categories, remain under development. The standalone brake kit is not sold because a physical effect has not been proven.
- GT4 missions, B-Spec, GT4 licence tests and unavailable GT4 courses are not part of this port. PSP licences remain in use.

The v0.27.2 game volume has been played on PSP Go. Beta.1 keeps that volume byte-identical and its new cover has been checked on PSP Go. A complete beta.1 career acceptance run and testing on other PSP models remain open.

## Download and install

Use the [patch selector](https://memetrix.github.io/gran-turismo-psp-career/) to pick your original USA ISO and download the matching `.xdelta`, then apply it with the free [Delta Patcher](https://deltapatcher.net/) for Windows or macOS. The ISO stays on your device during the check. Three USA image variants are supported; the [installation guide](https://github.com/Memetrix/gran-turismo-psp-career/blob/main/INSTALL.md) also lists their CRC32 values for manual selection. The smaller ZIP remains available as a command-line alternative for the originally supported image. **The downloads contain no game ISO or save file.**

The European `UCES01245` version is not supported in this beta. European support is planned for the full release.

- Finished ISO SHA-256: `1219e55d1fc0352ade90b2853c09de0441990a46407032acdc76c2adcabd31e6`
- USA UMD v2.00 `.xdelta` SHA-256: `172864242fc36f38bfd6e133451c901545d526020630e1bdea1b3c955b72f86f`
- USA UMD v1.00 `.xdelta` SHA-256: `d0fc7e8c58c975dd24cb00b0def3cc57f1aeff1c20e1f12355af15245fd9cb3b`
- Originally supported USA v2.00 `.xdelta` SHA-256: `6b03d3ef892adebaf3f600df9da935dcb916d96fb179be720fb31081af65d62f`
- Release ZIP SHA-256: `fdd66d63bff2f7674c20b431068b096f2dde6726ec5adea649cdf29d44c70949`
