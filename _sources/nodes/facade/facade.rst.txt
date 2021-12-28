===========
Facade Node
===========

This node can combine floors into a facade style. You can imagine floors as rows
in 2D array. So this node takes different rows and combine them together.
Read details in :doc:`/data_structure`.

The node can generate either infinite or finite facades. This properties can be
applied differently to facade length and height. Facade is infinite along length
if its floors are infinite. Facade is infinite along height if it has Fill
floor and Height parameter is equal 0. In all other cases a facade is finite.

Inputs
------

Last
  Last floor

Fill
  Floor which should be used to cover facade between first and last floors if
  they were given

First
  Fist floor. This is first floor of a facade not a building. Some times a
  facade can start from a second floor and above, in this case the first floor
  will be used any way.

Properties
----------

Height
  This is 0 by default what means that it's equal to actual facade height.
  This value can be overridden and generated style will be shooter than actual
  facade. This parameter is useful to use with :doc:`/nodes/facade/join_facades`.

Length
  The same as the Height property but instead determines the length of the 
  style.

Remote floor properties
-----------------------

Scalable
  If true the floor will be scale along Z axis together with other scalable
  floors to fit total height of floors into facade height. If all floors are
  not scalable the facade may have gap in the top.

Examples
--------

.. figure:: /images/nodes/Facade.*
   :width: 700 px

   Example of generating facade with first, fill and last floors.