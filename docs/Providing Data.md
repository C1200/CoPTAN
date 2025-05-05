# Providing Data

If you're interested: look into the documents related to NaPTAN, as this dataset is based on that. If information supplied here is incorrect, please correct me and provide your information in the correct way.

Please make sure to specify what type of stop/station you are providing. You may provide multiple stops of the same type in one issue.

## For Public Railways

The main `9100` prefixed entries are provided somewhat automatically. Should there be an issue, please notify me through the issues tab.

However, you may provide extra location information for (larger) stations. For this, you will need to open an issue with the following information:
- an `ATCOCode` - must start with your local ATCOPrefix (not `910`), followed with a `0`, followed by the station's up to 7 digit code (found in the `910` prefixed code), followed with a number `0`-`9` (`0` being the primary entrance/concourse/etc.)
- an `Indicator` - what does the coordinates point to? E.g. `Main Entrance`
- `PositionX` and `PositionZ` - what is the position?

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
