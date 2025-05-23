# Schema

The database provides the following information:

- `ATCOCode` - The unique alphanumeric code for a stop
- `CommonName` - The name of the stop
- `ShortCommonName` (nullable) - The shortened name of a stop
- `Indicator` (nullable) - This differentiates stops with the same `CommonName` (adj, o/s, opp, northbound, Bay 1, etc.)
- `Landmark` (nullable) - Could be used as an alternative to the `CommonName`
- `Street` (nullable) - Street name
- `LocalityCode` (nullable, but shouldn't be) - Primary Locality (town/city/village) ID
- `LocalityName` (nullable, but shouldn't be) - Primary Locality Name
- `ParentLocalityCode` (nullable)
- `ParentLocalityName` (nullable)
- `GrandParentLocalityCode` (nullable)
- `GrandParentLocalityName` (nullable)
- `Bearing` (nullable) - Which way the stop faces
- `PositionX` - X Coordinate
- `PositionZ` - Y Coordinate
- `StopType` - Stop Type

## Indicators

- `adj` - adjacent
- `o/s` - outside
- `opp` - opposite
- `nr` - near
- `Platform`, `Bay`, etc. followed by a number/letter
- A short stop identifier, examples of this can be found in big cities such as London

More may be acceptable

## Bearings

- Cardinal: `N`, `S`, `E`, `W`
- Intercardinal: `NE`, `SE`, `SW`, `NW`

## Stop Types

| Stop Type | Description                             | Global Prefix | Grouping Entry |
| --------- | --------------------------------------- | ------------- | -------------- |
| BCT       | Bus/Coach/Trolleybus stop               | -             | No             |
| RSE       | Rail Station Entrance                   | -             | No             |
| RLY       | Railway Interchange Area                | 910           | Yes            |
| RPL       | Railway Platform                        | 910           | No             |
| TMU       | Tram/Metro/Underground Entrance         | -             | No             |
| MET       | Tram/Metro/Underground Interchange Area | 940           | Yes            |
| PLT       | Tram/Metro/Underground Platform         | 940           | No             |
