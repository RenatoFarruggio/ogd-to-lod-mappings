## RML Mapping: Luftqualität Station Basel-Binningen

Stündliche Messungen der automatischen Wetterstation Basel-Binningen.

### Source Information
- **CSV Source:** https://data.bs.ch/api/explore/v2.1/catalog/datasets/100051/exports/csv?&use_labels=false&delimiter=%2C
- **Context/Metadata Files:** `dcat.ttl`, `fields.json`
- **Base URI:** `https://ld.bs.ch/cube/`

### Mapping Structure

**Dimensions:**
- `datum_zeit` (temporal) - granularity: hour
- `spatial_coverage` (spatial)

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
| 2021-02-04T05:00:00+00:00 | 04.02.2021 06:00 | 40.0 | 29.3 | 4.8 | 1.6 | 13398.4 | 0.2 | 0.0 | 0.0 | 1.3 | 30.0 | 5.3 |
| 2021-02-04T14:00:00+00:00 | 04.02.2021 15:00 | 48.1 | 21.2 | 9.3 | 3.5 | 14468.5 | 0.2 | 0.0 | 139.3 | 0.7 | 25.8 | 10.5 |
| 2021-02-04T19:00:00+00:00 | 04.02.2021 20:00 | 28.9 | 34.3 | 9.2 | 5.1 | 13834.9 | 0.5 | 0.0 | 0.0 | 1.4 | 35.1 | 8.9 |
| 2021-02-04T23:00:00+00:00 | 05.02.2021 00:00 | 29.0 | 27.3 | 9.9 | 6.4 | 10604.9 | 0.4 | 0.0 | 0.0 | 1.2 | 27.8 | 8.2 |
| 2021-02-05T00:00:00+00:00 | 05.02.2021 01:00 | 20.4 | 32.7 | 10.2 | 7.0 | 11886.7 | 0.5 | 0.0 | 0.0 | 2.4 | 33.2 | 7.7 |
| 2021-02-05T01:00:00+00:00 | 05.02.2021 02:00 | 7.7 | 32.9 | 13.7 | 10.2 | 11219.0 | 0.8 | 0.0 | 0.0 | 1.6 | 34.9 | 6.3 |
| 2021-02-05T03:00:00+00:00 | 05.02.2021 04:00 | 6.1 | 27.1 | 13.7 | 10.5 | 10250.2 | 0.8 | 0.0 | 0.0 | 1.0 | 28.8 | 5.5 |
| 2021-02-05T04:00:00+00:00 | 05.02.2021 05:00 | 6.5 | 23.1 | 12.1 | 9.3 | 8616.8 | 0.6 | 0.0 | 0.0 | 0.8 | 24.8 | 5.5 |
| 2021-02-05T05:00:00+00:00 | 05.02.2021 06:00 | 6.4 | 28.5 | 11.6 | 8.6 | 9776.5 | 0.6 | 0.0 | 0.2 | 1.5 | 31.5 | 6.0 |
| 2021-02-05T06:00:00+00:00 | 05.02.2021 07:00 | 3.2 | 34.8 | 11.7 | 8.2 | 12318.3 | 0.5 | 0.0 | 0.0 | 1.9 | 44.1 | 6.2 |
| 2021-02-05T07:00:00+00:00 | 05.02.2021 08:00 | 3.0 | 37.7 | 12.5 | 8.3 | 14651.7 | 0.5 | 0.0 | 1.2 | 2.3 | 54.9 | 6.4 |
| 2021-02-05T09:00:00+00:00 | 05.02.2021 10:00 | 6.8 | 32.7 | 15.4 | 9.0 | 16616.3 | 0.6 | 0.0 | 65.3 | 2.6 | 61.7 | 6.8 |
| 2021-02-05T13:00:00+00:00 | 05.02.2021 14:00 | 20.5 | 32.3 | 19.3 | 13.9 | 18069.4 | 0.7 | 0.0 | 239.7 | 2.9 | 58.8 | 12.1 |
| 2021-02-05T14:00:00+00:00 | 05.02.2021 15:00 | 17.8 | 38.0 | 20.4 | 12.0 | 17118.4 | 0.6 | 0.0 | 141.0 | 2.8 | 58.9 | 12.7 |
| 2021-02-05T17:00:00+00:00 | 05.02.2021 18:00 | 16.5 | 43.0 | 13.9 | 8.9 | 13016.6 | 0.7 | 0.0 | 2.7 | 1.3 | 47.4 | 12.0 |
| 2021-02-05T21:00:00+00:00 | 05.02.2021 22:00 | 2.7 | 39.9 | 21.6 | 21.7 | 9330.5 | 1.0 | 0.0 | 0.2 | 0.4 | 46.0 | 8.0 |
| 2021-02-06T00:00:00+00:00 | 06.02.2021 01:00 | 13.5 | 29.3 | 18.4 | 18.0 | 4414.7 | 0.7 | 0.0 | 0.5 | 0.3 | 30.0 | 7.5 |
| 2021-02-06T01:00:00+00:00 | 06.02.2021 02:00 | 13.5 | 27.0 | 18.6 | 18.2 | 4396.2 | 0.7 | 0.0 | 1.0 | 0.3 | 27.1 | 7.6 |
| 2021-02-06T02:00:00+00:00 | 06.02.2021 03:00 | 7.4 | 33.0 | 20.2 | 19.6 | 5725.7 | 0.8 | 0.0 | 0.3 | 0.5 | 35.0 | 7.3 |
| 2021-02-06T08:00:00+00:00 | 06.02.2021 09:00 | 5.9 | 22.4 | 18.2 | 17.0 | 8847.9 | 0.7 | 0.0 | 29.2 | 1.2 | 35.1 | 5.1 |

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

ex:observation-set cube:observation ex-obs:2021-02-04T05%3A00%3A00%2B00%3A00_Basel-Binningen,
    ex-obs:2021-02-04T14%3A00%3A00%2B00%3A00_Basel-Binningen, ex-obs:2021-02-04T19%3A00%3A00%2B00%3A00_Basel-Binningen .

ex-obs:2021-02-04T05%3A00%3A00%2B00%3A00_Basel-Binningen a cube:Observation;
  ex-property:RAUM ex-code:Basel-Binningen;
  ex-property:ZEIT "2021-02-04T05:00:00+00:00"^^xsd:dateTime;
  ex-property:cpc_1_cm3 13398.4;
  ex-property:ec_ug_m3 0.2;
  ex-property:no2_ug_m3 29.3;
  ex-property:nox_ug_m3_eq_no2 30.0;
  ex-property:o3_ug_m3 40.0;
  ex-property:pm10_ug_m3 4.8;
  ex-property:pm2_5_ug_m3 1.6;
  ex-property:prec_mm 0.0;
  ex-property:rad_w_m2 0.0;
  ex-property:so2_ug_m3 1.3;
  ex-property:temp_c 5.3 .

ex-obs:2021-02-04T14%3A00%3A00%2B00%3A00_Basel-Binningen a cube:Observation;
  ex-property:RAUM ex-code:Basel-Binningen;
  ex-property:ZEIT "2021-02-04T14:00:00+00:00"^^xsd:dateTime;
  ex-property:cpc_1_cm3 14468.5;
  ex-property:ec_ug_m3 0.2;
  ex-property:no2_ug_m3 21.2;
  ex-property:nox_ug_m3_eq_no2 25.8;
  ex-property:o3_ug_m3 48.1;
  ex-property:pm10_ug_m3 9.3;
  ex-property:
... (truncated)
```

---
_Generated by [OGD to LOD](https://github.com/opendatabs/ogd-to-lod)_
