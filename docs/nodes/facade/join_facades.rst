=================
Join Facades Node
=================

This can combine several facades into one by putting them on top of each other.
Also you can think about the work of this node as adding rows into a table where
rows are floors and table is final facade.

This node can join facades in different ways. If a facade does not have Fill
floor it takes all its available facades (first and last floors). If a facade
has Fill floor the join node will calculate available space for that facade.

Inputs
------

Facade
  Repeatable socket which expects sequence of facades to be join.

Remote facade properties
------------------------

Join size
  This parameter is used if more than two given facades has Fill floors. In
  that case available space for each facade is calculated according to this
  parameter. For example if one facade has this parameter equal 1 and another
  facade has the parameter equal 2 than 1 facade will take 1/3 of available
  space and the second 2/3.

Examples
--------
