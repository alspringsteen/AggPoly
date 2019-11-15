# AggPoly
AggPoly (aggregate polygons) is a QGIS3-Plugin for aggregation and generalization of polygons within a certain distance with respect to barriers.
The algorithm takes a polygon and optional barrier layer (of any geometry type) and returns features that link areas, which are within the specified distance. If a barrier layer is chosen, the new features don't cross the features of the barrier layer.

## Example
[example image](example.jpeg)

## Performance
The algorithm relies on polygon vertices.
Consequently, complex input polygons with a high vertex count have a huge performance impact!
If possible and without substantial downside, simplify / generalise your input.

## Issues
A lot!
This is still a prove-of-concept!