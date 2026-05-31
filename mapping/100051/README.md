## RML Mapping: Luftqualität Station Basel-Binningen

Stündliche Messungen der automatischen Wetterstation Basel-Binningen.

### Source Information
- **CSV Source:** https://data.bs.ch/api/explore/v2.1/catalog/datasets/100051/exports/csv?&use_labels=true&delimiter=%2C
- **Context/Metadata Files:** `dcat.ttl`, `fields.json`
- **Base URI:** `https://ld.bs.ch/cube/`

### Mapping Structure

- The columns `datum_zeit` (UTC timestamp) and `timestamp_text` (local time string) are mapped as temporal dimensions to uniquely identify each observation and support different time representations.
- All pollutant and meteorological columns (`o3_ug_m3`, `no2_ug_m3`, `pm10_ug_m3`, `pm2_5_ug_m3`, `cpc_1_cm3`, `ec_ug_m3`, `prec_mm`, `rad_w_m2`, `so2_ug_m3`, `nox_ug_m3_eq_no2`, `temp_c`) are mapped as measures, reflecting the quantitative hourly observations captured at the station.
- No data columns were dropped; every column is either a key dimension or a measure.
- No explicit hierarchies or aggregation levels were defined, as each row represents a unique observation for a specific timestamp.
- All property URIs were consistently constructed using sanitized column names and the dataset-scoped `ex-property:` prefix to ensure valid RDF, future-proof reuse, and harmonization.

**Dimensions:**
- `datum_zeit` (temporal) - granularity: hour
- `timestamp_text` (temporal) - granularity: hour

**Measures:**
- `o3_ug_m3` (μg/m3)
- `no2_ug_m3` (μg/m3)
- `pm10_ug_m3` (μg/m3)
- `pm2_5_ug_m3` (μg/m3)
- `cpc_1_cm3` (1/cm3)
- `ec_ug_m3` (μg/m3)
- `prec_mm` (mm)
- `rad_w_m2` (W/m2)
- `so2_ug_m3` (μg/m3)
- `nox_ug_m3_eq_no2` (μg/m3)
- `temp_c` (°C)

### CSV Preview

| datum_zeit | timestamp_text | o3_ug_m3 | no2_ug_m3 | pm10_ug_m3 | pm2_5_ug_m3 | cpc_1_cm3 | ec_ug_m3 | prec_mm | rad_w_m2 | so2_ug_m3 | nox_ug_m3_eq_no2 | temp_c |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2019-07-22T17:00:00+00:00 | 22.07.2019 18:00 | 124.0 | 6.6 | 11.4 | 6.4 | 8949.9 | 0.2 | 0.0 | 300.2 | 0.5 | 6.8 | 29.7 |
| 2019-07-23T00:00:00+00:00 | 23.07.2019 01:00 | 70.3 | 9.6 | 12.9 | 7.3 | 6705.9 | 0.3 | 0.0 | 0.0 | 0.4 | 10.0 | 19.6 |
| 2019-07-23T02:00:00+00:00 | 23.07.2019 03:00 | 55.6 | 11.4 | 10.8 | 7.6 | 6898.1 | 0.3 | 0.0 | 0.0 | 0.4 | 11.7 | 17.7 |
| 2019-07-23T10:00:00+00:00 | 23.07.2019 11:00 | 117.2 | 10.6 | 13.4 | 8.7 | 10748.9 | 0.2 | 0.0 | 793.3 | 0.6 | 12.0 | 29.4 |
| 2019-07-23T14:00:00+00:00 | 23.07.2019 15:00 | 137.6 | 4.2 | 10.4 | 7.7 | 5371.2 | 0.1 | 0.0 | 826.3 | 0.2 | 4.4 | 33.8 |
| 2019-07-23T19:00:00+00:00 | 23.07.2019 20:00 | 132.8 | 10.9 | 14.3 | 9.1 | 9508.7 | 0.2 | 0.0 | 34.7 | 0.6 | 11.0 | 31.1 |
| 2019-07-23T23:00:00+00:00 | 24.07.2019 00:00 | 82.5 | 20.0 | 18.8 | 12.1 | 10085.1 | 0.4 | 0.0 | 0.0 | 1.3 | 20.1 | 24.3 |
| 2019-07-24T00:00:00+00:00 | 24.07.2019 01:00 | 72.9 | 18.4 | 18.9 | 12.2 | 8879.9 | 0.4 | 0.0 | 0.0 | 1.4 | 18.7 | 22.5 |
| 2019-07-24T03:00:00+00:00 | 24.07.2019 04:00 | 78.1 | 14.5 | 14.9 | 11.7 | 8621.4 | 0.3 | 0.0 | 0.0 | 1.5 | 14.7 | 21.2 |
| 2019-07-24T07:00:00+00:00 | 24.07.2019 08:00 | 64.9 | 39.8 | 23.0 | 12.7 | 16867.6 | 0.6 | 0.0 | 345.8 | 1.5 | 48.2 | 23.8 |
| 2019-07-24T12:00:00+00:00 | 24.07.2019 13:00 | None | None | 17.8 | 10.4 | 5424.8 | 0.2 | 0.0 | 899.7 | None | None | 34.5 |
| 2019-07-24T13:00:00+00:00 | 24.07.2019 14:00 | 143.6 | 3.4 | 15.7 | 9.3 | 5352.2 | 0.2 | 0.0 | 889.0 | 0.6 | 4.4 | 35.5 |
| 2019-07-24T14:00:00+00:00 | 24.07.2019 15:00 | 145.6 | 3.8 | 13.1 | 8.0 | 7181.9 | 0.1 | 0.0 | 824.3 | 0.5 | 3.8 | 36.1 |
| 2019-07-24T16:00:00+00:00 | 24.07.2019 17:00 | 162.6 | 5.3 | 13.0 | 8.3 | 5766.0 | 0.2 | 0.0 | 555.8 | 0.5 | 5.5 | 36.5 |
| 2019-07-24T18:00:00+00:00 | 24.07.2019 19:00 | 155.4 | 5.6 | 16.8 | 9.7 | 4170.4 | 0.2 | 0.0 | 192.5 | 0.5 | 5.8 | 35.1 |
| 2019-07-24T21:00:00+00:00 | 24.07.2019 22:00 | 85.8 | 21.2 | 26.5 | 14.3 | 12599.2 | 0.6 | 0.0 | 0.0 | 0.8 | 21.8 | 26.1 |
| 2019-07-24T22:00:00+00:00 | 24.07.2019 23:00 | 95.8 | 11.4 | 26.1 | 13.5 | 7760.3 | 0.4 | 0.0 | 0.0 | 0.5 | 11.6 | 24.6 |
| 2019-07-25T00:00:00+00:00 | 25.07.2019 01:00 | 82.8 | 16.3 | 17.7 | 11.9 | 8404.3 | 0.4 | 0.0 | 0.0 | 1.2 | 16.5 | 24.3 |
| 2019-07-25T05:00:00+00:00 | 25.07.2019 06:00 | 67.1 | 28.4 | 16.4 | 12.4 | 10869.2 | 0.4 | 0.0 | 47.7 | 2.6 | 29.3 | 21.4 |
| 2019-07-25T06:00:00+00:00 | 25.07.2019 07:00 | 57.2 | 42.9 | 19.7 | 13.3 | 15976.5 | 0.7 | 0.0 | 146.5 | 2.0 | 47.7 | 21.7 |

### RDF Preview

```turtle
@prefix : <http://mapping.example.com/> .
@prefix csvw: <http://www.w3.org/ns/csvw#> .
@prefix cube: <https://cube.link/> .
@prefix d2rq: <http://www.wiwiss.fu-berlin.de/suhl/bizer/D2RQ/0.1#> .
@prefix dc: <http://purl.org/dc/terms/> .
@prefix ex: <https://ld.bs.ch/cube/100051/> .
@prefix ex-code: <https://ld.bs.ch/cube/code/> .
@prefix ex-obs: <https://ld.bs.ch/cube/100051/observation/> .
@prefix ex-property: <https://ld.bs.ch/cube/property/> .
@prefix fnml: <http://semweb.mmlab.be/ns/fnml#> .
@prefix fno: <https://w3id.org/function/ontology#> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix rml: <http://w3id.org/rml/> .
@prefix schema: <http://schema.org/> .
@prefix void: <http://rdfs.org/ns/void#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

ex:observation-set cube:observation ex-obs:2019-07-22T17%3A00%3A00%2B00%3A00_22.07.2019%2018%3A00,
    ex-obs:2019-07-23T00%3A00%3A00%2B00%3A00_23.07.2019%2001%3A00, ex-obs:2019-07-23T02%3A00%3A00%2B00%3A00_23.07.2019%2003%3A00 .

ex-obs:2019-07-22T17%3A00%3A00%2B00%3A00_22.07.2019%2018%3A00 a cube:Observation;
  ex-property:ZEIT "2019-07-22T17:00:00+00:00"^^xsd:dateTime;
  ex-property:ZEIT_text "22.07.2019 18:00";
  ex-property:cpc_1_cm3 8949.9;
  ex-property:ec_ug_m3 0.2;
  ex-property:no2_ug_m3 6.6;
  ex-property:nox_ug_m3_eq_no2 6.8;
  ex-property:o3_ug_m3 124.0;
  ex-property:pm10_ug_m3 11.4;
  ex-property:pm2_5_ug_m3 6.4;
  ex-property:prec_mm 0.0;
  ex-property:rad_w_m2 300.2;
  ex-property:so2_ug_m3 0.5;
  ex-property:temp_c 29.7 .

ex-obs:2019-07-23T00%3A00%3A00%2B00%3A00_23.07.2019%2001%3A00 a cube:Observation;
  ex-property:ZEIT "2019-07-23T00:00:00+00:00"^^xsd:dateTime;
  ex-property:ZEIT_text "23.07.2019 01:00";
  ex-property:cpc_1_cm3 6705.9;
  ex-property:ec_ug_m3 0.3;
  ex-property:no2_ug_m3 9.6;
  ex-property:nox_ug_m3_eq_no2 10.0;
  ex-property:o3_ug_m3 70.3;
  ex-property:pm10_
... (truncated)
```

---
_Generated by [OGD to LOD](https://github.com/opendatabs/ogd-to-lod)_
