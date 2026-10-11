Data
Large files are not stored in git. Each source is listed here with its link and where our copy lives.
Desk check done on 11 Oct 2026. Status changes to ✅ only after a team member downloads a real sample.
#	Source	Used for	ID / Link	Resolution	Coverage / last update	License	Our copy (Drive / GEE asset)	Status
1	Sentinel-2 L2A Harmonized	Vegetation (NDVI)	`COPERNICUS/S2_SR_HARMONIZED`	10 m (B4, B8)	2017-03 → ongoing (latest image 11 Oct 2026)	Copernicus Sentinel Data Terms		🔎 available
2	Dynamic World V1	Land-cover classes (trees, grass, built, bare…)	`GOOGLE/DYNAMICWORLD/V1`	10 m	2015-06 → near real-time (11 Oct 2026)	CC-BY 4.0		🔎 available
3	Landsat 8/9 Collection 2 Level-2 (ST_B10)	Land-surface temperature	`LANDSAT/LC09/C02/T1_L2` + `LANDSAT/LC08/C02/T1_L2`	30 m delivered (thermal sensor native 100 m)	L9: 2021-10 → 8 Oct 2026	Public domain (credit USGS)		🔎 available
4	WorldPop R2025A — KSA, constrained	Population density	sau_pop_2025_CN_100m_R2025A_v1.tif	~100 m	Years 2015–2030; file dated 2 Aug 2025; alpha release, may change	CC-BY 4.0		🔎 available (53 MB → Drive, not git)
5a	Riyadh Municipality Geoportal — neighbourhoods	Spatial unit (official)	mapservice.alriyadh.gov.sa/geoportal	Polygons	Neighbourhood layer viewable; download not offered publicly	Needs written permission		🟡 send request
5b	Tabaqat `geocoding-cng` — `sa_districts.parquet`	Spatial unit (fallback)	source.coop/tabaqat/geocoding-cng	Polygons (189 districts in Riyadh municipality)	v0.4.2	Not stated — confirm before use		🔁 fallback candidate
5c	OpenStreetMap	Spatial unit (fallback)	—	—	KSA import covers regions & governorates only, not neighbourhoods	ODbL		❌ not suitable
Status: ⬜ not started · 🔎 confirmed online (desk check) · 🟡 requested · ✅ sample downloaded · 🔁 fallback ready · ❌ not suitable
Notes
Earth Engine account: register a Cloud project as noncommercial (university email). Since 27 Apr 2026 noncommercial projects get a monthly quota; the free Community tier = 150 EECU-hours/month per project. Keep exports to Riyadh only, and each member can use their own project.
Cloud masking for Sentinel-2: use Cloud Score+ (`GOOGLE/CLOUD_SCORE_PLUS/V1/S2_HARMONIZED`). The old `QA60` band has a gap (2022-01 → 2024-02).
Landsat LST in Kelvin: `ST_B10 × 0.00341802 + 149.0`, then − 273.15 for °C.
Required citation: Dynamic World — Brown et al. (2022), Scientific Data 9, 251, doi:10.1038/s41597-022-01307-4.
