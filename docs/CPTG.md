# CPTG
The CPTG (Community Public Transport Gazetteer) provides regions for use with the main CoPTAN database.

## Schema
- `LocalityCode` - Locality (town/city/village) ID 
- `LocalityName`
- `ParentLocalityCode` (nullable) - Parent Locality ID (there may be more parents above this)
- `ParentLocalityName` (nullable)
- `ATCOPrefix` (nullable) - Local ATCO Prefix, should be used if a global ATCO is not applicable
- `PositionX` (nullable)  - X Coordinate
- `PositionZ` (nullable)  - Y Coordinate
