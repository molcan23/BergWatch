# BergWatch




## Datasets

Datasets can be downloaded by two APIs.

### Copernicus Marine Service API Access
```
python -m motuclient --motu https://nrt.cmems-du.eu/motu-web/Motu --service-id ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011-TDS --product-id cmems_mod_arc_phy_anfc_nextsim_hm --longitude-min -179.9898 --longitude-max 179.9795 --latitude-min 41.5692 --latitude-max 89.991 --date-min "2021-11-11 23:30:00" --date-max "2021-11-11 23:30:00" --variable latitude --variable longitude --variable siconc --variable sisnthick --variable sithick --variable stereographic --variable vxsi --variable vysi --out-dir <OUTPUT_DIRECTORY> --out-name <OUTPUT_FILENAME> --user <USERNAME> --pwd <PASSWORD>
```

New Data Request: 7am, 6 nov
[Data | Copernicus Marine](https://resources.marine.copernicus.eu/product-download/ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011)
[a | Copernicus Marine](https://resources.marine.copernicus.eu/product-download/ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011)
**![](https://lh6.googleusercontent.com/y2seU1RJYwcbZ-GzvA4FQDyNkNAy-AoCgQmOzQj_tkMaycq66J5fFlZIeQQxUiwEpprmP5iseDSfIFePZy6FGJdnNs0vXJktrmQdxVUinRnO2GxgLSWSIL4FUOdKkps9LHUmXrDj)**

**![](https://lh4.googleusercontent.com/bb9IzzNlVViLqXbCrKEi7lJY6JpIbe9cPHfrJAO3Gyca_cDvwnmh99HXtJYVGPEilu8YJj4iSZVgHsyDiF8mrWNf7m_rF9zTHd7Heu1zTZCfZQIUYcQ2orK5a1ZNcRNRdn2D-ASp)**

**![](https://lh3.googleusercontent.com/IN-MqPAdEsmeeTevucMpXkCa4BfgjuiuYbjOPD25QtzhA2tWm5079asPlE365Ch0ugPmu8NVSXQebDS7iQQLRvn6XETfcRxQG0XZCwmwTEnuyW-yjPcGiEQaoXAvBcNNU0EL1rUE)**

```
python -m motuclient --motu https://nrt.cmems-du.eu/motu-web/Motu --service-id ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011-TDS --product-id cmems_mod_arc_phy_anfc_nextsim_hm --longitude-min -29 --longitude-max -17.87 --latitude-min 63.3 --latitude-max 72 --date-min "2021-11-01 00:30:00" --date-max "2021-11-12 23:30:00" --variable latitude --variable longitude --variable siconc --variable sithick --variable vxsi --variable vysi --out-dir <OUTPUT_DIRECTORY> --out-name <OUTPUT_FILENAME> --user <USERNAME> --pwd <PASSWORD>
```

### Wekeo API Access

```
{
	"datasetId": "EO:MO:DAT:ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011:cmems_mod_arc_phy_anfc_nextsim_hm",
	"boundingBoxValues": [
		{
			"name": "bbox",
			"bbox": [
				-115.02485937500002,
				67.16813278215082,
				85.21401562500002,
				84.40332895737387
			]
		}
	],
	"dateRangeSelectValues": [
		{
			"name": "position",
			"start": "2018-11-01T00:00:00.000Z",
			"end": "2021-11-05T00:00:00.000Z"
		}
	],
	"multiStringSelectValues": [
		{
			"name": "variable",
			"value": [
				"vysi"
			]
		}
	],
	"stringChoiceValues": [
		{
			"name": "service",
			"value": "ARCTIC_ANALYSISFORECAST_PHY_ICE_002_011-TDS"
		},
		{
			"name": "product",
			"value": "cmems_mod_arc_phy_anfc_nextsim_hm"
		}
	]
}
```
