# Licensed health tourism facilities in Turkey (2026)

A clean, machine-readable list of the **680 hospitals and medical centres** that the Turkish Ministry of Health has authorised to treat international patients (health tourism), across **55 provinces**.

The Ministry publishes this list only as PDF files. This dataset converts it into CSV and JSON so it can be searched, filtered and joined with other data.

- **Source:** Turkish Ministry of Health, Department of Health Tourism – [authorised health facilities list](https://shgmturizmdb.saglik.gov.tr/TR-25360/yetkili-saglik-tesisleri-ve-araci-kuruluslar.html) (accessed 2026-10-29)
- **Maintained by:** [TurkClinics Guide](https://www.turkclinicsguide.com/open-data) – an independent, multilingual guide to clinics in Turkey
- **Licence:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) – free to reuse with attribution

## Files

| File | Format | Rows |
|---|---|---|
| `data/licensed-health-tourism-facilities-turkey.csv` | CSV, UTF-8 with BOM, comma-separated | 680 |
| `data/licensed-health-tourism-facilities-turkey.json` | JSON | 680 |

## Fields

| Field | Description |
|---|---|
| `name` | Official registered name of the facility, as published by the Ministry (Turkish) |
| `type` | Facility type as published (Turkish), normalised to 7 categories |
| `type_en` | English translation of `type` |
| `province` | Province (il) |
| `district` | District (ilçe), empty when not given in the source |
| `address` | Address as published |

Phone numbers from the source are intentionally **not** included.

## Facilities by type

| Type | Count |
|---|---|
| Private hospital | 348 |
| Private medical centre | 135 |
| Public hospital | 109 |
| Public university hospital | 40 |
| Private (foundation) university hospital | 36 |
| Public dental hospital | 11 |
| Private dental hospital | 1 |

## Top provinces

| Province | Facilities |
|---|---|
| İstanbul | 224 |
| Ankara | 68 |
| İzmir | 59 |
| Antalya | 43 |
| Bursa | 18 |
| Kocaeli | 18 |
| Gaziantep | 17 |
| Konya | 14 |

## How to use it

- **Patients:** before booking, ask the clinic for its *official registered name* and check that it appears in this list. Many brands operate under a different legal name or inside a partner hospital.
- **Researchers and journalists:** the distribution of authorised facilities by province and type.
- **Developers:** join on `name` or geocode the `address` field.

## Notes and limitations

- This list covers **hospitals and medical centres**. Authorised private practices (muayenehane) and polyclinics are published by the Ministry in separate lists and are not included here.
- Being on the list means the facility is authorised for health tourism. It is **not** a quality rating or a recommendation.
- Names and addresses are reproduced as published; the Ministry may update its list at any time. Always check the [official source](https://shgmturizmdb.saglik.gov.tr/TR-25360/yetkili-saglik-tesisleri-ve-araci-kuruluslar.html).
- Clinic profiles, treatment guides and published prices: [turkclinicsguide.com](https://www.turkclinicsguide.com/).

## Citation

> TurkClinics Guide (2026). *Licensed health tourism facilities in Turkey* [Data set]. Based on Turkish Ministry of Health data (accessed 2026-10-29). https://www.turkclinicsguide.com/open-data
