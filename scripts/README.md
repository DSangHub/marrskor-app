# Scoring workbook generators

These scripts live in the working copy used to build `Marrskor_Skor_Model_v1.xlsx`.

Yellow cells + blue numbers are inputs. Black cells are formulas.

```bash
python3 scripts/build_skor_workbook.py
python3 scripts/add_ownership_sheet.py
```

The generated `.xlsx` is gitignored.

Ownership rules (also in PRODUCT.md):

- VIN capture + checksum + NHTSA vPIC decode (specs only)
- Registration/title photo with street address blocked before storage
- No silent DMV owner-name lookup
- CA DMV Wallet / state credentials when the owner presents them
