# ez_banklogos

Indian bank logos by IFSC code, for EZFinanz apps. Same layout as
praveenpuglia/indian-banks, so the app's `BankLogoWidget` only needs its base URL changed.

## Layout

```
assets/logos/<ifsc-code-lowercase>/symbol.png
```

Examples: `hdfc`, `sbin`, `icic`, `utib` (Axis), `kkbk` (Kotak), `ubin` (Union), `idib` (Indian Bank), `cnrb` (Canara).
`banks.json` maps each code to the bank name and the original source file.

## URLs (after pushing and tagging, e.g. v1.0.0)

```
https://cdn.jsdelivr.net/gh/<org>/ez_banklogos@v1.0.0/assets/logos/<code>/symbol.png
https://raw.githubusercontent.com/<org>/ez_banklogos/v1.0.0/assets/logos/<code>/symbol.png
```

Point the app at a tag, never `main`, so logo changes ship only on purpose.

## Source and license

- Logo files: nkscoder/indian-banks (MIT), converted to PNG (at most 256 px). See LICENSE and LICENSE-nkscoder.
- 20 more (v1.1.0): rendered from praveenpuglia/indian-banks SVGs (no license; see "Added in v1.1.0").
- Bank names / IFSC codes: razorpay/ifsc (MIT).
- Logos are the banks' trademarks, used only to identify the bank.

## Added in v1.1.0

20 banks not in the nkscoder set were rendered (256 px PNG) from praveenpuglia/indian-banks' `symbol.svg`:
`abbl airp clbl ctcb esmf fdrl ibbk jsfb kvbl mshq nbad nesf rabo sbld sibl smcb stcb sury unba utks`
(incl. Federal Bank `fdrl`, Karur Vysya `kvbl`, South Indian `sibl`, Jana SFB `jsfb`, Utkarsh SFB `utks`).

Note: praveenpuglia/indian-banks has **no license file**, so these 20 files come without an explicit reuse
grant (`banks.json` marks their source). Replace them with the banks' official logos when possible.

Images are at most 256 px; many are 96x96. Replace any that look soft with the bank's official SVG/PNG
(`symbol.svg` is also picked up by the app first).
