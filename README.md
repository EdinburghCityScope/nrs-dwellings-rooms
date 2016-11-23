# nrs-dwellings-rooms
Number of dwellings by number of rooms within the dwelling.

Data on Council Tax band, type of dwelling and number of rooms are obtained from the Assessors’ Portal. The Assessors are, amongst other things, responsible for valuing each dwelling in Scotland for the purposes of assigning it to a Council Tax Band.

Dwellings - This is the total number of dwellings on the Council Tax valuation list (excluding free-standing private lock-ups and garages). A 'dwelling' refers to the accommodation itself, for example a house or a flat, and includes second homes that are not let out commercially. Caravans count as dwellings if they are someone’s main home.

Number of Rooms - This is defined as the number of habitable rooms (usually bedrooms and living rooms). This is different to the census definition, which includes kitchens. There may be some differences between different Assessors' areas in the way in which this information is recorded. For example, differences could arise in the treatment of open plan areas, dining rooms, kitchens and kitchenettes. Assessors are only able to reflect physical changes and alterations to dwellings once they have been sold and a reconsideration of the banding has taken place therefore this information may not always represent the most up-to-date position. Information on the number of rooms is not available for most dwellings in Shetland. No information is separately available for dwellings with seven or more rooms in Dumfries and Galloway.

Summary statistics on dwellings in Scotland are published annually in 'Estimates of Households and Dwellings in Scotland', which is available on the NRS website at the following link: http://www.nrscotland.gov.uk/statistics-and-data/statistics/statistics-by-theme/housholds/household-estimates

Statistics provided by National Records of Scotland:  http://statistics.gov.scot/data/dwellings-rooms

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/nrs-dwellings-rooms.git
```

Install npm dependencies

```
cd nrs-dwellings-rooms
npm install
```

Run the API (from the nrs-dwellings-rooms directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
