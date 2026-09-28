# static-maps

Finished map exports from Millcreek GIS (City of Millcreek, Utah). Each file can
be linked or embedded directly by its raw GitHub URL (see below).

This repo holds images only. There is no source data, map project, or code.

## Contents

| File | Map | Size (px) |
| --- | --- | --- |
| `ANSI - 11x17 - Landscape - AADT with Labels UDOT 2023 Data - 082224.png` | Annual Average Daily Traffic (UDOT 2023 data) | 4250 × 2750 |
| `ANSI - 11x17 - Landscape - Alcohol Spacing for ULCT - 080824 - QR Final.png` | Alcohol Spacing 2024: 300 ft / 600 ft buffers around community locations | 4250 × 2750 |
| `ANSI - 11x17 - Landscape - Promise - Poverty Levels 2024 - ACS Data - 062024v4.png` | Population under 200% of the federal poverty level, by census tract (ACS) | 4420 × 2860 |
| `ANSI - 11x17 - Landscape - RSL Map August 2024 w private roads.png` | Pavement Conditions 2024: remaining service life (RSL), with private roads | 4250 × 2750 |
| `ANSI - 11x17 - Landscape - Sensitive Lands Overview 042125v2png.png` | Sensitive Lands Overview | 4250 × 2750 |
| `Full GSD Boundary with Muni Boundaries043025.jpg` | Granite School District boundary with municipalities | 5950 × 3850 |
| `Full High School GSD Boundary with Muni Boundaries 050125.jpg` | Granite School District high school boundaries with municipal overlay | 10200 × 6600 |
| `Full Junior High GSD Boundary with Muni Boundaries 050125.jpg` | Granite School District junior high boundaries with municipal overlay | 10200 × 6600 |
| `futurelanduseforweb031325.jpg` | Future Land Use (General Plan) | 10800 × 7200 |

The six-digit number in most filenames is a date (`MMDDYY`) from when that
version was made.

## Linking to a map

Use the raw file URL, with spaces encoded as `%20`:

```text
https://raw.githubusercontent.com/buschbrian/static-maps/main/futurelanduseforweb031325.jpg
https://raw.githubusercontent.com/buschbrian/static-maps/main/ANSI%20-%2011x17%20-%20Landscape%20-%20Sensitive%20Lands%20Overview%20042125v2png.png
```

Renaming or deleting a file breaks every link that points to it, so publish an
updated map under a new filename and remove the old one only once nothing
links to it.

## Adding a map

1. Export from ArcGIS Pro as PNG or JPEG.
2. Install the pre-commit hooks once per clone: `pre-commit install`.
3. Commit and push.

The pre-commit hook rejects files larger than 5 MB (`--maxkb=5120`). Several of
the existing PNGs are larger than that and were added before the hook existed,
so export new maps as JPEG or compress them before committing.

## Disclaimer

These maps are for informational purposes only. See the disclaimer printed on
each map.
