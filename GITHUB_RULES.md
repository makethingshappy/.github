# Instruction 2. Changing the makethingshappy GitHub repositories

**1. Scope.** Repositories IoTextra-Digital, IoTextra-Analog, IoTextra-Combo, IoTsmart, IoTbase and `.github`. What applies to each is given in section 13.

**2. Write permission.** Claude does not write to GitHub. Claude prepares the file and shows "before / after"; the owner writes it.

**3. What a push triggers.**
- `overview.md` or `*-logo.svg` → Overview Sync immediately rewrites the README and the product card.
- Compatibility tables in `.github` → MTH Sync (changes other repositories) and Shopify Sync (changes site pages).
- Docs Sync is started manually. A dry run (`apply` unchecked: changes nothing, shows the future card HTML and README) is at the owner's discretion.

**4. Module folder structure.**
- Module folder root: `README.md`, `SKU.md`, `overview.md`, `*-logo.svg`, `examples/`, revision folders `v.X.XX/`.
- Revision folder: `docs/`, `hardware/`, `media/`, `synergy.yml`, `host-map.yaml`. `synergy.yml` and `host-map.yaml` are not moved.
- Module folder names are the Short Names. They must not be renamed.

**5. File names.** Docs Sync finds documents by name: `docs/…Datasheet…pdf`, `hardware/…Schematic…pdf`, `docs/…Pinout…(png|jpg|pdf)`, `hardware/*.step`. Example: `IoTextra MOSFET2 - Datasheet - Rev.3-02.pdf`.

**6. README.** The blocks between the markers OVERVIEW, PRODUCT, SYNERGY, SOFTWARE and `docs-sync:badges` are generated automatically and are not edited by hand. Only text outside markers is edited manually.

**7. overview.md.** First line: `# <Title>`. Then the overview lines, separated by blank lines. The last line is shown in small grey type. Links only as `<a href>`.

**8. synergy.yml.** Every SKU on sale is listed in exactly one list (`direct` or `spacer_or_cable`) for each target, otherwise Docs Sync stops.

**9. Language.** English only, no Cyrillic in any file.

**10. PDF.** All PDFs (datasheets, schematics) are placed in GitHub by the owner.

**11. Procedure.**
1. Read the current version of the file from the repository.
2. Prepare the file and show "before / after".
3. After the owner's upload, check the workflow result and the outcome in the card or README.

**12. Stop.** The action is stopped and reported if: the file cannot be read; a workflow failed; the result on the site does not match the expected one; the change does not fit this Instruction.

**13. What applies in each repository.**

| Repository | Applies | Does not apply (yet) |
|---|---|---|
| IoTextra-Digital | the whole Instruction | — |
| IoTsmart, IoTbase | sections 1–3, 6 (OVERVIEW only), 7, 9–12, 14; from section 4 — module folder names | Docs Sync, `synergy.yml`, sections 5, 8; structure of section 4 (folders still contain `overview.svg`, `software.svg`, `placeholder.txt`; IoTbase RPi has no `overview.md`) |
| IoTextra-Analog, IoTextra-Combo | same as IoTsmart and IoTbase | same; to be brought to the Digital scheme by the next revision |
| `.github` | sections 1–3, 9–12, 14 | sections 4–8 |

**14. Exception.** The Instructions themselves are changed only on the owner's direct command.
