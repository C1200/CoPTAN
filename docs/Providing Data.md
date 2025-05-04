# Providing Data

Please make sure to specify what type of stop/station you are providing. You may provide multiple stops of the same type in one issue.

## For Public Railways

Create an issue with the following information:
- an `ATCOCode` (optional) - must start with `9100` and can end with up to 8 capitalised alphanumeric characters
- a `CommonName` - just the station's name (no Rail/Train Station suffixes please)
- a `Street` - what street is the main entrance on?
- a `LocalityName` hierarchy - what town, city, district, cardinal direction is it part of?
- `PositionX` and `PositionZ` - what is the position of the main entrance?

## For Bus & Tram

> Important: an entry should be made for every single:
> - Bus stop
> - Bus station bay
> - Tram platform
>
> No grouping of Bus & Tram access nodes is permitted

Create an issue with the following information:
- an `ATCOCode` (optional) - must start with your local ATCOPrefix, followed by a `0`, followed by up to 8 capitalised alphanumeric characters (if not sure of your prefix, do not provide an ATCOCode)
- a `CommonName`
  - for tram: suffix with `Tram Stop`
  - for bus: usually the name of the adj/opp street
- a `Street` - what street is the stop on?
- a `LocalityName` hierarchy - what town, city, district, cardinal direction is it part of?
- an `Indicator` (optional) - what is the direction of travel?
- `PositionX` and `PositionZ` - what is the position of the stop?
- a `StopType` - look into NaPTAN stop types, or just provide one in plain english
