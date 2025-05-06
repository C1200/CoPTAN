# Providing Data

Explanations for some fields may be omitted. If editing the CSV file yourself,
please check what should go in the omitted fields before submitting a pull
request.

## Bus

There should be one entry per physical bus stop:

- If there's two bus stops close together, one for each direction: submit them
  individually
- If there's a line of bus stops all for one direction: submit them individually
- If there's a bus station which has multiple bays: submit each bay individually

You'll need to provide the following data for each stop:

- an `ATCOCode`, see [Making an ATCOCode](Making%20an%20ATCOCode.md#bus)
- a `CommonName`, usually the name of:
  - a nearby street
  - a nearby landmark or other place of interest
  - *other's are acceptable*
- an `Indicator` if there are multiple stops in the same area with the same
  name. See [Schema#Indicators](Schema.md#indicators) for examples
- a `Landmark` if there's a nearby place of interest like a railway station
- the `Street`, the name of the street the stop is actually on, should be given
  in the unabbreviated form
- the `LocalityCode`, found in CPTG
- the `PositionX` and `PositionZ`

## Public Railways

Data which populates the 910 ATCO prefix is semi-automatically provided.
Therefore, it should not be manually edited or added.

Rail station entrances may be manually added. The following information is
needed:
- an `ATCOCode`, see [Making an ATCOCode](Making%20an%20ATCOCode.md#public-railways)
- a `CommonName`, the same common name as the main entry
- an `Indicator` for example: Main Entrance
- the `Street` the entrance is on
- the `PositionX` and `PositionZ`

## Trams and Other Metro Systems

One entry must be provided per platform (with StopType = PLT) and one more entry
must be provided (with StopType = MET) to group everything together. On top of
this entrances (with StopType = TMU) can optionally be provided.

For METs:
- an `ATCOCode`, see [Making an ATCOCode](Making%20an%20ATCOCode.md#trams-and-other-metro-systems)
- a `CommonName`, usually the name of:
  - a nearby street
  - a nearby landmark or other place of interest
  - *other's are acceptable*
- a `Landmark` if there's a nearby place of interest like a railway station
- the `Street`, the name of the street the stop is actually on, should be given
  in the unabbreviated form
- the `LocalityCode`, found in CPTG
- the `PositionX` and `PositionZ`

For PLTs and TMUs: follow the guidance on entrances for [Public Railways](#public-railways)
