# Hawaii ZIP Codes

A reference CSV of all 139 Hawaii ZIP codes with island, county, neighborhood, P.O. box flag, and special-purpose type.

## File

**`hawaii_zipcodes.csv`** — one row per ZIP code.

| Column | Description |
|--------|-------------|
| `zipcode` | 5-digit ZIP code |
| `island` | Physical island (Oahu, Maui, Molokai, Lanai, Hawaii, Kauai, Wake Island) |
| `county` | Administrative county (Oahu, Maui, Hawaii, Kauai). Note: Maui County includes Molokai and Lanai; Oahu (Honolulu County) administratively includes Wake Island. |
| `neighborhood` | Neighborhood or area name (e.g., "Kailua, Kaneohe", "Hilo", "Lahaina"). For single-entity ZIPs, includes the entity in parentheses (e.g., "Honolulu (HECO)"). |
| `pobox` | `1` if the ZIP is P.O. box only, `0` if it serves street addresses |
| `type` | Blank for standard ZIPs. `military` for military installations, `unique` for single-entity corporate/government ZIPs, `territory` for Wake Island. |

## Coverage

- **87 standard community ZIP codes** across all major islands
- **12 Honolulu P.O. box ZIPs** (968xx series serving Downtown Honolulu)
- **7 military installations** — JBPHH, Hickam Housing, Wheeler, Fort Shafter, Tripler, Camp Smith, MCBH Kaneohe Bay
- **7 single-entity ZIPs** — Hawaiian Electric, Hawaiian Telcom, Board of Water Supply, University of Hawaii, Bank of Hawaii, First Hawaiian Bank, IRS
- **3 small Honolulu ZIPs** (96827, 96835, 96838)
- **1 territory** — Wake Island (96898)

## Island vs. County

Hawaii's counties don't map 1:1 to islands. The `island` column captures the physical island while `county` captures the administrative unit:

| ZIP | Island | County | Neighborhood |
|-----|--------|--------|-------------|
| 96729 | Molokai | Maui | Molokai |
| 96742 | Molokai | Maui | Molokai |
| 96748 | Molokai | Maui | Molokai |
| 96757 | Molokai | Maui | Molokai |
| 96770 | Molokai | Maui | Molokai |
| 96763 | Lanai | Maui | Lanai |
| 96898 | Wake Island | Oahu | Wake Island |

## Sources

Compiled from Hawaii Department of Taxation administrative records and USPS ZIP code reference data.
