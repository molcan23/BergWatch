# BergWatch

Imagine floating by on top of an iceberg, in the middle of the ocean; the northern lights covering the picturesque sky and it all while being in the middle of the arctic ocean. We invite you to turn this dream into reality, all the while supporting the local arctic community and the environment.
 
We develop a new exciting way to experience the arctic and to experience our planet. In this, we provide two-tier services: an exclusive arctic paradise for our premium customers and a youth arctic climate showcase bringing our youth close to the arctic, where the brunt of climate change is often felt the worst. Our hope is, by influencing these two key customer groups: premium customers who will likely be people of influence and changemakers, and the youth who are the future of our planet, we induce a significant climate conversation.
 
We envision to organize ourselves as a technology company, partnering ourselves up with existing Nordic travel companies. Our introduction to the market brings added value to the industry with our technological intelligence: offering a unique iceberg vacation experience, detecting likely northern light events or meteor showers, etc.
 
A big proportion of the profit from the premium users will be redistributed to the community, to uplift the living of the indigenous community and to protect the Arctic environment. Utmost care will be taken in our venture to ensure minimal impact on the environment, using natural amenities as much as possible; and our customer experiences will be designed in a way to bring climate awareness and hopefully induce lasting behavioral change to tackle the climate crisis.
 
## 🚀 EU space technologies
We exploit the Copernicus Marine Service Arctic Ocean Sea Ice Analysis and Forecast data, to detect large floating sea ice, and to detect the trajectory of these sea ice. The selected sea ice, whose safety criteria have been satisfied and whose trajectory is well understood will be used for our arctic experience venture.
 
## ❄️ Connecting the Arctic
We are solving the “safe passage at sea” hackathon challenge while creating a new exciting tourism industry around it; by detecting and implementing sea ice travel ventures on large and safe sea ice trajectories. 
 
Further, our business model will be designed in a way to contribute to the local arctic community and the environment.
 
### Team 
**Samuel Molčan** (*GIS, Coding*): Ph.D. candidate in Computer Engineering; Experienced programmer/machine learning expert.

**Amin Shakya** (*GIS, Coding*): Has a double master’s degree in disaster risk management; interested in the tech-for-good market space.

**Ivan Mrekaj** *(Society-science interface*): Climate and environmental scientist with a forestry background, focused on phenology, drought in forest ecosystems, and climate change.

**Tatiana Telecká** (*Business Development, Marketing*): Mechanical engineer with expert experience in manufacturing production, assembly, and marketing.

**Pavel Kubíček** (*Business development, Marketing*): Student of trade and business with a specialization in agricultural technology.


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
