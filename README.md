# MKV Series Catalog

Public community catalog for MKV Chapter Cutter series definitions.

The app reads `series-catalog/series-manifest.json`, then downloads `series-catalog/series-definitions.json` and imports approved entries into the local SQLite database.

## Suggest an entry

Use the `Eintrag vorschlagen` button in MKV Chapter Cutter. It opens a prefilled GitHub issue with the selected episode as JSON.

## Maintainer update flow

1. Review issues labeled `series-suggestion`.
2. Copy accepted JSON entries into `series-catalog/series-definitions.json`.
3. Increase `catalog_version` and update `updated_at`.
4. Recalculate the SHA-256 of `series-definitions.json`.
5. Update `series-catalog/series-manifest.json` with the same version/date and hash.
