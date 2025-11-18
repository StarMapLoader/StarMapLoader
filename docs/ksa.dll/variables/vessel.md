# Vessels
## Disclaimer
More variables are needed, as not all variables are in here yet, just the important ones

## Body/Vessel Variables Related to Movement

- double: Vehicle.Orbit.Apoapsis
- double: Vehicle.Orbit.Eccentricity
- double: Vehicle.Orbit.Inclination
- double: Vehicle.Orbit.LongitudeOfAscendingNode
- Orbit: Vehicle.Orbit.Orbit

- double: Vehicle.Orbit.SemiMajorAxis
- double: Vehicle.Orbit.SemiMinorAxis
- double: Vehicle.Orbit.Period
## Body/Vessel Specs
- bool: Vehicle.IsTarget
- string: Vehicle.Class

## Time
- SimTime: Vehicle.Orbit.GetElapsedTimeSincePeriapsis
- SimTime: Vehicle.Orbit.TimeAtPeriapsis