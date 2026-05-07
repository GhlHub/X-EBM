# Repository Guidance

## Layout

- `doc/`: PDF datasheets and reference documents.
- `release/`: generated release artifacts such as Gerber ZIPs.
- `x-ebm.dch`: primary schematic/design file.
- `x-ebm-01.dip`: related project/design file.
- `bom1.xlsx`: bill of materials spreadsheet.

## File Handling

- Keep vendor PDFs in `doc/` instead of the repository root.
- Keep generated release bundles in `release/`.
- Preserve lowercase naming for the main design file: `x-ebm.dch`.
- Avoid adding macOS metadata files such as `._*` files.

## Git

- Prefer rename/move operations over delete-and-recreate so history stays readable.
- Review binary changes carefully before committing, especially updates under `release/`.
