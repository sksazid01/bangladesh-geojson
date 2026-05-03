# Bangladesh GeoJSON

Bangladesh administrative boundary data including Divisions, Districts, Upazilas, and Post Offices in JSON/GeoJSON format.

---

## Files

### `All_GeoInfo.json`
A single consolidated file containing all geographic data: **country**, **divisions**, **districts**, **upazilas**, and **postcodes**.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/All_GeoInfo.json
```

**Structure:**
- `countries` — 1 entry (Bangladesh) with `id`, `name`, `bn_name`, `lat`, `lng`
- `divisions` — 8 divisions with `id`, `country_id`, `name`, `bn_name`, `lat`, `lng`
- `districts` — 64 districts with `id`, `division_id`, `name`, `bn_name`, `lat`, `lng`
- `upazilas` — 494 upazilas with `id`, `district_id`, `name`, `bn_name`
- `postcodes` — 1349 entries with `division_id`, `district_id`, `upazila`, `postOffice`, `postCode`

---

### `Nested_Division_Zila_Upazila_Post.json`
Hierarchical (nested) structure: each division contains its zilas, each zila contains its upazilas, and each upazila contains its post offices.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/Nested_Division_Zila_Upazila_Post.json
```

---

### `bd-divisions.json`
8 divisions with `id`, `name`, `bn_name`, `lat`, `long`.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/bd-divisions.json
```

---

### `bd-districts.json`
64 districts mapped to divisions, with `id`, `division_id`, `name`, `bn_name`, `lat`, `long`.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/bd-districts.json
```

---

### `bd-upazilas.json`
494 upazilas mapped to districts, with `id`, `district_id`, `name`, `bn_name`.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/bd-upazilas.json
```

---

### `bd-postcodes.json`
1349 post office entries with `division_id`, `district_id`, `upazila`, `postOffice`, `postCode`.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/bd-postcodes.json
```

---

### `bangladesh.geojson`
GeoJSON boundary data for Bangladesh.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/bangladesh.geojson
```

---

### `dhaka-city.json`
GeoJSON boundary data for Dhaka city.

**JSON Endpoint:**
```
https://raw.githubusercontent.com/sksazid01/bangladesh-geojson/main/dhaka-city.json
```

---

## Data Summary

| File | Records | Description |
|---|---|---|
| `All_GeoInfo.json` | All-in-one | Country, Divisions, Districts, Upazilas, Postcodes |
| `Nested_Division_Zila_Upazila_Post.json` | Nested | Hierarchical Division → Zila → Upazila → Post |
| `bd-divisions.json` | 8 | Divisions |
| `bd-districts.json` | 64 | Districts |
| `bd-upazilas.json` | 494 | Upazilas |
| `bd-postcodes.json` | 1349 | Post Offices & Postcodes |
| `bangladesh.geojson` | — | Bangladesh boundary (GeoJSON) |
| `dhaka-city.json` | — | Dhaka city boundary (GeoJSON) |
