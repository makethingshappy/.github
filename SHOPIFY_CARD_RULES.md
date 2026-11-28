# Instruction 1. Changing a Shopify product card

**1. Scope.** Any content (field) of any product card on makethingshappy.io.

**2. Write permission.** Claude writes to a card only after the owner's approval. Each field is approved separately: "write the Title" and "write the tags" are two different approvals. One approval covers one write.

**3. Structure of the description.**

| Block | Source | Written by |
|---|---|---|
| OVERVIEW | `<Module>/overview.md` | Overview Sync, immediately on push |
| BADGES | Digital: `.github/IOTEXTRA_*_COMPATIBILITY.md`; others: `*-logo.svg` | Digital: Docs Sync; others: Overview Sync |
| SOFTWARE | `.github/IOTEXTRA_*_COMPATIBILITY.md` | Docs Sync (Digital only) |
| SYNERGY | `<Module>/v.X.XX/synergy.yml` | Docs Sync (Digital only) |
| DOCS (Links) | revision PDFs; the revision is taken from the variant SKUs | Docs Sync (Digital only) |
| COMPARE | comparisons in GitHub | manually |
| Description text, variants table, Key Specifications, Applications and everything else outside markers | exists only in the card, no copy anywhere | manually |

A marker block is delimited by the comments `<!-- NAME_START -->` … `<!-- NAME_END -->`.

**4. Fields the workflows depend on.**
- **Title** must end with `<Family> <module folder name>`, e.g. `IoTextra MOSFET2` or `IoTsmart ESP32-S3`. The workflows find the product by this ending. If both the Title and the overview change, the Title is changed first, then `overview.md` is uploaded.
- **Variant SKUs** (Digital) define the revision whose documents Docs Sync shows under Links. Every SKU on sale must be listed in `synergy.yml`.
- **Collection** defines which repository syncs the product: `digital-iotextra`, `iotsmart`, `iotbase`, etc.

**5. Procedure.**
1. Read the field fresh from Shopify. Never take it from a saved file, an old chat or a cache.
2. If a description change falls inside a marker block, change the source in GitHub per Instruction 2, not the card.
3. Outside markers, change only the required fragment in the freshly read copy.
4. Show "before / after" and get approval for this field.
5. After writing, read the field again and check: only the approved change was made; the description has the same set of markers; there is no Cyrillic.
6. Report what was changed.

**6. Prohibited.**
- Overwriting the whole description from any copy, or suggesting that the owner do so.
- Deleting, renaming or moving markers.
- Editing the content of a marker block directly in Shopify.
- Introducing design elements that are not in the approved cards without the owner's agreement.
- Using `<style>`. Using HTML comments other than markers.
- Writing Cyrillic.
- SEO title longer than 70 characters, meta description longer than 160.

**7. Stop.** The action is stopped and reported if: the field cannot be read; markers are damaged or their set differs from the expected one; a workflow failed; the change does not fit this Instruction.

**8. Exception.** This Instruction is changed only on the owner's direct command.
