# US severe weather warning counts by state, county and city

How many tornado, severe thunderstorm and flash flood warnings the National Weather Service issued for every US state, county, DC and Puerto Rico, and for 3,614 cities, each year from 2008, with tornado counts since 1950. Also winter storm, extreme cold, heat, wildfire, air quality, hurricane, high wind and flood counts.

These are the same numbers as the state, county and city pages on [kinwarn.com](https://kinwarn.com/), as CSV files you can reuse under CC BY 4.0. Warnings through 2026-10-19.

## Files

| File | Rows |
|---|---|
| [`data/all-states.csv`](data/all-states.csv) | 6,886: 50 states, DC and Puerto Rico, 3,220 counties, 3,614 cities |
| `data/<state>.csv` | one state with its counties and cities; the first line is a comment with the method |

Each row has `type` (state, county or city), name, state, county, the county's NWS code (`county_ugc`), center point and population, then the counts. Column names carry their years, for example `tornado_warnings_2016_2025` or `flash_flood_warnings_2019`.

## How the numbers are counted

National Weather Service warnings via the Iowa Environmental Mesonet through 2026-10-19; tornadoes from the Storm Prediction Center (1950-2025) and NWS Storm Events through 2026-06-30. Counties and the state: warnings that listed the county. Cities: warnings whose outline covered the city center point set by the Census Bureau; population: Census 2025 estimate (unincorporated communities: GeoNames). WEA columns: warnings that set off Wireless Emergency Alerts on phones in the warned area (tornado; severe thunderstorm tagged destructive; flash flood tagged considerable or catastrophic, at issue or in an update whose outline covered the city center or touched the county). Winter columns (July 1 to June 30 winters): winter storm, blizzard, ice storm, lake effect snow and snow squall warnings; extreme cold warnings including wind chill warnings; cities: the forecast zones holding the center point (snow squall: the outline), counties: zones covering at least a tenth of the county (snow squall: warnings that listed the county). Heat columns (calendar years): extreme heat warnings including excessive heat warnings, and heat advisories, matched the same way. Wildfire columns: National Interagency Fire Center wildfires (not prescribed burns) that started within 50 km of the center, acres for the whole fire. AQI column: days the county's highest EPA monitor reading was above 100 (cities: their county; blank = no monitor). Storm columns: storms that brought a hurricane, tropical storm or storm surge warning (each storm once per warning type, even when two NWS offices warned the place; storm surge warnings since 2017); high wind warnings; both by forecast zone, matched like the heat columns. Flood columns: river (FL) and areal (FA) flood warnings, counted like flash flood warnings (outline at the city center; county listed); a warning cancelled before it began does not count.

The full method, with examples, is on [kinwarn.com/about](https://kinwarn.com/about#how-we-count). These are counts of past warnings, not warnings in effect now. For warnings where you are, follow your local [National Weather Service](https://www.weather.gov/) office.

## Sources

- National Weather Service warnings, through the [Iowa Environmental Mesonet](https://mesonet.agron.iastate.edu/) archive
- Tornadoes: [Storm Prediction Center](https://www.spc.noaa.gov/wcm/) database and NWS [Storm Events](https://www.ncdc.noaa.gov/stormevents/)
- Places: US Census Bureau Gazetteer and population estimates, GeoNames
- Wildfires: National Interagency Fire Center; air quality: US EPA

## License and citation

The counts are licensed under [CC BY 4.0](LICENSE). Credit Kinwarn with a link to the page the numbers came from, for example:

> Kinwarn, "Oklahoma tornado warnings", kinwarn.com/oklahoma. National Weather Service data via the Iowa Environmental Mesonet.

## States

| State | Page | CSV | Counties | Cities |
|---|---|---|---|---|
| Alabama | [kinwarn.com/alabama](https://kinwarn.com/alabama) | [alabama.csv](data/alabama.csv) | 67 | 69 |
| Alaska | [kinwarn.com/alaska](https://kinwarn.com/alaska) | [alaska.csv](data/alaska.csv) | 30 | 0 |
| Arizona | [kinwarn.com/arizona](https://kinwarn.com/arizona) | [arizona.csv](data/arizona.csv) | 15 | 66 |
| Arkansas | [kinwarn.com/arkansas](https://kinwarn.com/arkansas) | [arkansas.csv](data/arkansas.csv) | 75 | 40 |
| California | [kinwarn.com/california](https://kinwarn.com/california) | [california.csv](data/california.csv) | 58 | 245 |
| Colorado | [kinwarn.com/colorado](https://kinwarn.com/colorado) | [colorado.csv](data/colorado.csv) | 64 | 62 |
| Connecticut | [kinwarn.com/connecticut](https://kinwarn.com/connecticut) | [connecticut.csv](data/connecticut.csv) | 8 | 36 |
| Delaware | [kinwarn.com/delaware](https://kinwarn.com/delaware) | [delaware.csv](data/delaware.csv) | 3 | 11 |
| District of Columbia | [kinwarn.com/district-of-columbia](https://kinwarn.com/district-of-columbia) | [district-of-columbia.csv](data/district-of-columbia.csv) | 1 | 1 |
| Florida | [kinwarn.com/florida](https://kinwarn.com/florida) | [florida.csv](data/florida.csv) | 67 | 317 |
| Georgia | [kinwarn.com/georgia](https://kinwarn.com/georgia) | [georgia.csv](data/georgia.csv) | 159 | 115 |
| Hawaii | [kinwarn.com/hawaii](https://kinwarn.com/hawaii) | [hawaii.csv](data/hawaii.csv) | 4 | 26 |
| Idaho | [kinwarn.com/idaho](https://kinwarn.com/idaho) | [idaho.csv](data/idaho.csv) | 44 | 13 |
| Illinois | [kinwarn.com/illinois](https://kinwarn.com/illinois) | [illinois.csv](data/illinois.csv) | 102 | 226 |
| Indiana | [kinwarn.com/indiana](https://kinwarn.com/indiana) | [indiana.csv](data/indiana.csv) | 92 | 89 |
| Iowa | [kinwarn.com/iowa](https://kinwarn.com/iowa) | [iowa.csv](data/iowa.csv) | 99 | 41 |
| Kansas | [kinwarn.com/kansas](https://kinwarn.com/kansas) | [kansas.csv](data/kansas.csv) | 105 | 38 |
| Kentucky | [kinwarn.com/kentucky](https://kinwarn.com/kentucky) | [kentucky.csv](data/kentucky.csv) | 120 | 45 |
| Louisiana | [kinwarn.com/louisiana](https://kinwarn.com/louisiana) | [louisiana.csv](data/louisiana.csv) | 64 | 56 |
| Maine | [kinwarn.com/maine](https://kinwarn.com/maine) | [maine.csv](data/maine.csv) | 16 | 12 |
| Maryland | [kinwarn.com/maryland](https://kinwarn.com/maryland) | [maryland.csv](data/maryland.csv) | 24 | 121 |
| Massachusetts | [kinwarn.com/massachusetts](https://kinwarn.com/massachusetts) | [massachusetts.csv](data/massachusetts.csv) | 14 | 91 |
| Michigan | [kinwarn.com/michigan](https://kinwarn.com/michigan) | [michigan.csv](data/michigan.csv) | 83 | 101 |
| Minnesota | [kinwarn.com/minnesota](https://kinwarn.com/minnesota) | [minnesota.csv](data/minnesota.csv) | 87 | 103 |
| Mississippi | [kinwarn.com/mississippi](https://kinwarn.com/mississippi) | [mississippi.csv](data/mississippi.csv) | 82 | 41 |
| Missouri | [kinwarn.com/missouri](https://kinwarn.com/missouri) | [missouri.csv](data/missouri.csv) | 115 | 88 |
| Montana | [kinwarn.com/montana](https://kinwarn.com/montana) | [montana.csv](data/montana.csv) | 56 | 6 |
| Nebraska | [kinwarn.com/nebraska](https://kinwarn.com/nebraska) | [nebraska.csv](data/nebraska.csv) | 93 | 17 |
| Nevada | [kinwarn.com/nevada](https://kinwarn.com/nevada) | [nevada.csv](data/nevada.csv) | 17 | 15 |
| New Hampshire | [kinwarn.com/new-hampshire](https://kinwarn.com/new-hampshire) | [new-hampshire.csv](data/new-hampshire.csv) | 10 | 14 |
| New Jersey | [kinwarn.com/new-jersey](https://kinwarn.com/new-jersey) | [new-jersey.csv](data/new-jersey.csv) | 21 | 157 |
| New Mexico | [kinwarn.com/new-mexico](https://kinwarn.com/new-mexico) | [new-mexico.csv](data/new-mexico.csv) | 33 | 21 |
| New York | [kinwarn.com/new-york](https://kinwarn.com/new-york) | [new-york.csv](data/new-york.csv) | 62 | 196 |
| North Carolina | [kinwarn.com/north-carolina](https://kinwarn.com/north-carolina) | [north-carolina.csv](data/north-carolina.csv) | 100 | 95 |
| North Dakota | [kinwarn.com/north-dakota](https://kinwarn.com/north-dakota) | [north-dakota.csv](data/north-dakota.csv) | 53 | 9 |
| Ohio | [kinwarn.com/ohio](https://kinwarn.com/ohio) | [ohio.csv](data/ohio.csv) | 88 | 187 |
| Oklahoma | [kinwarn.com/oklahoma](https://kinwarn.com/oklahoma) | [oklahoma.csv](data/oklahoma.csv) | 77 | 46 |
| Oregon | [kinwarn.com/oregon](https://kinwarn.com/oregon) | [oregon.csv](data/oregon.csv) | 36 | 1 |
| Pennsylvania | [kinwarn.com/pennsylvania](https://kinwarn.com/pennsylvania) | [pennsylvania.csv](data/pennsylvania.csv) | 67 | 87 |
| Puerto Rico | [kinwarn.com/puerto-rico](https://kinwarn.com/puerto-rico) | [puerto-rico.csv](data/puerto-rico.csv) | 78 | 30 |
| Rhode Island | [kinwarn.com/rhode-island](https://kinwarn.com/rhode-island) | [rhode-island.csv](data/rhode-island.csv) | 5 | 11 |
| South Carolina | [kinwarn.com/south-carolina](https://kinwarn.com/south-carolina) | [south-carolina.csv](data/south-carolina.csv) | 46 | 56 |
| South Dakota | [kinwarn.com/south-dakota](https://kinwarn.com/south-dakota) | [south-dakota.csv](data/south-dakota.csv) | 66 | 14 |
| Tennessee | [kinwarn.com/tennessee](https://kinwarn.com/tennessee) | [tennessee.csv](data/tennessee.csv) | 95 | 67 |
| Texas | [kinwarn.com/texas](https://kinwarn.com/texas) | [texas.csv](data/texas.csv) | 254 | 275 |
| Utah | [kinwarn.com/utah](https://kinwarn.com/utah) | [utah.csv](data/utah.csv) | 29 | 63 |
| Vermont | [kinwarn.com/vermont](https://kinwarn.com/vermont) | [vermont.csv](data/vermont.csv) | 14 | 4 |
| Virginia | [kinwarn.com/virginia](https://kinwarn.com/virginia) | [virginia.csv](data/virginia.csv) | 133 | 71 |
| Washington | [kinwarn.com/washington](https://kinwarn.com/washington) | [washington.csv](data/washington.csv) | 39 | 0 |
| West Virginia | [kinwarn.com/west-virginia](https://kinwarn.com/west-virginia) | [west-virginia.csv](data/west-virginia.csv) | 55 | 14 |
| Wisconsin | [kinwarn.com/wisconsin](https://kinwarn.com/wisconsin) | [wisconsin.csv](data/wisconsin.csv) | 72 | 98 |
| Wyoming | [kinwarn.com/wyoming](https://kinwarn.com/wyoming) | [wyoming.csv](data/wyoming.csv) | 23 | 7 |

Made by [Kinwarn](https://kinwarn.com/), tornado, severe storm and flash flood alerts for your home and your family's homes.
