# GT PSP Career: Spec II — public beta 0.27.2-beta.1

GT Career adds a nine-hall career to **Gran Turismo PSP USA (UCUS98632 v2.00)**, based on the event structure and economy of GT4 Spec II 1.10. This is a beta, not a claim that every GT4 mechanism has been ported.

## Apply the patch

This beta ZIP is **not a standalone `.xdelta` file**. Delta Patcher cannot open it. Extract the ZIP and run the included `apply_patch.py` installer as shown below.

You need your own, unmodified USA UCUS98632 v2.00 ISO, Python 3.8 or newer, `xdelta3` on your PATH, the .NET 9 or 10 runtime, and about 5 GB of free disk space. The original ISO must have SHA-256:

`78d1b6855a268bd6480a6572977c3f4df4c438af11c751baeca14390819de435`

Keep the extracted beta bundle together. From a terminal inside its folder:

```sh
python3 apply_patch.py "/path/to/your/original.iso" "/path/to/GT-Career-SpecII-beta.iso"
```

On Windows, use `python` or `py` in place of `python3`. If `dotnet` is not on your PATH, add `--dotnet /path/to/dotnet`. The script patches individual game files, rebuilds the game volume, and checks the finished ISO against the SHA-256 in `manifest.json`. It never overwrites the original or an existing output. Copy the finished ISO to your PSP's `ISO` folder or open it in PPSSPP.

No game ISO, save file, or test profile is included in this release. Back up your savedata before trying a beta or updating from an older GT Career version. The career uses its own `UCUS98632-CAREER` slot; on first launch it copies the garage and credits from the stock `UCUS98632-GAMEDAT` slot when present. The stock slot is not overwritten. Changes in beta save formats may reset career progress while preserving the game's garage, credits, and licences.

## What is in this beta

- Nine career halls with 161 GT4-derived competitions, 42 continuation pages for long series, two PSP-specific lost-circuit events, and two clearly named hidden-course diagnostic events. The catalog has 763 career rounds and seven diagnostic rounds.
- Connected championships with shared points and rivals; Special Conditions uses two-car races.
- Buying and fitting engine upgrades, suspension, tyres, and applicable brake controls. Purchases survive saving and refitting. The purchase journal holds at most 192 tuned-car configurations.
- Segmented endurance races with saved progress. Timed marathons carry cumulative distance, the same entrants and rolling-start position between segments; the final prize depends on cumulative placing.
- A separate career save, repeatable event runs, prize cars, and a live `POS n/4` guide during timed marathon segments.

## Known beta limits

- When a new endurance segment starts near the finish line, the game's **best-lap display** can count the first partial lap as a very short lap. Marathon classification subtracts the segment's start position from distance, so this display error does not award a full lap.
- A full accumulated 24-hour race has not yet been completed as an acceptance run. Lap-based endurance scoring and some race-result edge cases are still being validated.
- The rolling-segment `POS n/4` HUD is an estimate during the race; the confirmed result uses lap count and position on the track.
- The hidden-course diagnostic events are experimental. They exist to test recovered tracks and may fail; do not use them as evidence of career completion.
- Native opponent configurations, pace balance across all classes, and the remaining GT4 tuning categories are still under development. Brake controls have a measured effect; a standalone brake kit has not been shown to change stopping performance.
- The v0.27.2 gameplay image has been played on PSP Go; this beta.1 image keeps that game volume byte-identical and its new cover has been checked on PSP Go. Other PSP models and a complete 24-hour session have not yet been accepted on hardware.

The `screenshots/` folder contains unscaled 480×272 frames from the PSP framebuffer in an isolated PPSSPP run of the exact beta.1 ISO. They are emulator captures, not photos of the hardware screen.

Report a problem with the console model or PPSSPP version, event and round, what happened, and whether it survives a cold launch. Do not post copyrighted ISO files or personal saves publicly. Source and licence notices are included separately with the release.
