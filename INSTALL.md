# Install GT Career: Spec II

You need your own unmodified **Gran Turismo PSP USA UCUS98632 v2.00** ISO. The patch does not include the game.

1. Download `GT-Career-SpecII-v0.27.2-beta.1.xdelta` from the [release page](https://github.com/Memetrix/gtpsp-career-spec-ii/releases/tag/v0.27.2-beta.1), plus the free [Delta Patcher](https://deltapatcher.net/) for Windows or macOS.
2. Make a copy of your original ISO. In Delta Patcher, choose the copy under **Original file**.
3. Choose the downloaded `.xdelta` under **XDelta patch** and click **Apply patch**. Delta Patcher changes the selected ISO copy. When it reports success, copy that ISO to your PSP's `ISO` folder or open it in PPSSPP.

These are screenshots from an actual installation; your file paths will differ.

![Original ISO and Spec II patch selected in Delta Patcher](screenshots/delta-patcher-ready.jpg)

![Delta Patcher confirming the patch was applied](screenshots/delta-patcher-success.jpg)

If Delta Patcher reports a checksum error, you have a different game version or a previously modified ISO. The required original SHA-256 is `78d1b6855a268bd6480a6572977c3f4df4c438af11c751baeca14390819de435`. Keep checksum validation on.

## Saves

Back up your savedata before trying the beta or updating from an older version. The career uses its own `UCUS98632-CAREER` save. On first launch it can copy your garage and credits from the stock `UCUS98632-GAMEDAT` save without overwriting it. Future beta updates may reset career progress while preserving the garage, credits and licences.

<details>
<summary>Smaller command-line patch (advanced)</summary>

The 81 MB ZIP on the release page is an alternative for users who prefer a smaller download. It is not a `.xdelta` file. It needs Python 3.8+, `xdelta3` on your PATH, the .NET 9 or 10 runtime and about 5 GB of free disk space. Extract the ZIP, then run this from a terminal inside its folder:

```sh
python3 apply_patch.py "/path/to/your/original.iso" "/path/to/GT-Career-SpecII-beta.iso"
```

On Windows, use `python` or `py` in place of `python3`. If `dotnet` is not on your PATH, add `--dotnet /path/to/dotnet`. This installer leaves the original ISO untouched.

</details>

For features and known beta limits, see the [release notes](RELEASE-NOTES-v0.27.2-beta.1.md). [Report a problem](https://github.com/Memetrix/gtpsp-career-spec-ii/issues) with the console model or PPSSPP version, event and round, and what happened.
