# CFU Calculator

Colony counts → CFU/mL, in a single self-contained HTML file.

**Live:** https://mbaffour.github.io/cfu-calculator/

- Name your samples and log replicates — colony count, dilution (any factor, any step), and volume plated per row. New replicates inherit the previous row's dilution and volume.
- Per-sample **mean ± SD and CV%** across countable replicates.
- Counts outside the countable window (30–300 per plate, 3–30 per spot) are flagged; mark a plate **TNTC** or **Excl** to drop it from the stats.
- All-zero samples report a **detection limit** (`< 1 colony at the least-diluted plate`) instead of a bogus mean.
- Export a real **.xlsx** workbook (Raw counts + Summary sheets, numbers stay numeric) or CSV — no libraries, the OOXML writer is built in.
- Zero dependencies, no network, autosaves to your browser's local storage. Works from `file://`.

CFU/mL = colonies × dilution factor<sup>step</sup> ÷ volume plated (mL).

Also available as the **CFU Counts** module inside
[Dilution Designer](https://mbaffour.github.io/dilution-designer/), where counts
can be captured into the lab notebook and included in workspace backups.
