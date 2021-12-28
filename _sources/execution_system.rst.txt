================
Execution system
================

You can think about the add-on as a custom modifier based on node editor
(similar to geometry nodes modifier). Except that you won't be able to find
it neither in list of modifiers nor in modifier stack because custom modifiers
are in BLender anti-features_ list. Instead, the :ref:`main panel <main_panel>`
can be found in Property panel (N) of viewport editor. It has similar interface
as Blender modifiers.

.. _anti-features: https://wiki.blender.org/wiki/Reference/AntiFeatures

For now there are only two events which force building style to be applied to
a base mesh:

- When :ref:`base mesh <base_geometry>` is edited in edit mesh. This will cause
  update only active object.
- When building style is edited. This will update all objects which use the
  node tree.

Both updates can be enabled/disabled via :ref:`main panel <main_panel>`.

.. note::

   Any other updates are not supported. For example shape are ignored. Also all
   modifiers are ignored. So you won't be able to generate procedural shapes
   for buildings. But probably this feature will be added in the future
   releases.

.. warning::

   For its work the add-on adds Geometry nodes modifier to the object receiving
   facade style. It's not recommended to edit its tree. In new versions the
   tree can be recreated from scratch without saving any changes in previous
   one.

.. warning::

   Also there is problem of copying an object with building style. When initial
   object is edited the copied object will repeat the shape of this changes.
   In order to make changes of the copy fully separate from initial object
   either building style tree should be updated (by dragging a link for
   example) or the copy should be put in edit mode.

.. todo add information about realtime editing problems (Ctrl+R)

.. _tree_editor:

-----------
Tree editor
-----------

In general the work in facade style editor is similar to work in any other
standard tree editors except a few things.

- Adding animation keys and drivers to the node properties is not supported.
  This is limitation of Blender and nothing can be done on the add-on side.
- Muting nodes currently is not supported. Can be implemented in
  the future but not before Blender 3.1 release.
- Node groups are not supported. Unfortunately during development of Geometry
  nodes project there was brought new problems (problem1_, problem2_, problem3_)
  which prevent from using node groups safely in add-ons. It also means that
  there are no custom properties per building. So there won't be node groups
  at list until crushing issues won't be fixed.

.. _problem1: https://developer.blender.org/T90233
.. _problem2: https://developer.blender.org/T88795
.. _problem3: https://developer.blender.org/T82812


.. _errors:

Errors
^^^^^^

During tree execution there can be some errors which prevents building being
updated. Errors are shown on the :ref:`main panel <main_panel>`. It can be some
low level error which message is not very helpful and can be considered as bug.
Or it can be a high level error:

- Size error
    It means that some of the panels has 0 height or 0 length. Panels can have
    0 length along any axis but not when it used to fill some space. For example
    a panel should has length if it is used to fill a floor.