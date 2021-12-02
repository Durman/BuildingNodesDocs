======================
Facade Attributes Node
======================

This node outputs facade attributes as fields. Read more about :ref:`fields`
and :ref:`facades`.

Outputs
-------

Left corner angle
  Angle between current facade and neighbour facade from left side. Unit of
  angle is radian. The straight angle between outputs 0 radians. Obtuse angles
  return positive values, reflex angles return negative values. It's possible
  that the same corner has multiple different angles in this case only one of
  them is taken into account.

Right corner angle
  The same as Left angle but this angle is determined by the current facade
  and facade from the right side.

Material index
  Index of a material slot which is assigned to faces of the facade. By default
  facades are split by border lines of different materials so one facade always
  has only one associated material index.

Index
  Index of the current facade. Also this can be considered as facade ID because
  indexing of facades does not have any particular order.

Length
  Distance between left and right corners.

Examples
--------
