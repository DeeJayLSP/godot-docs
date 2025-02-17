:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/AStarGrid2D.xml.

.. _class_AStarGrid2D:

AStarGrid2D
===========

**Inherits:** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`



Properties
----------

+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`Vector2<class_Vector2>`                      | :ref:`cell_size<class_AStarGrid2D_property_cell_size>`                 | ``Vector2(1, 1)``  |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`Heuristic<enum_AStarGrid2D_Heuristic>`       | :ref:`default_heuristic<class_AStarGrid2D_property_default_heuristic>` | ``0``              |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`DiagonalMode<enum_AStarGrid2D_DiagonalMode>` | :ref:`diagonal_mode<class_AStarGrid2D_property_diagonal_mode>`         | ``0``              |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`bool<class_bool>`                            | :ref:`jumping_enabled<class_AStarGrid2D_property_jumping_enabled>`     | ``false``          |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`Vector2<class_Vector2>`                      | :ref:`offset<class_AStarGrid2D_property_offset>`                       | ``Vector2(0, 0)``  |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+
| :ref:`Vector2i<class_Vector2i>`                    | :ref:`size<class_AStarGrid2D_property_size>`                           | ``Vector2i(0, 0)`` |
+----------------------------------------------------+------------------------------------------------------------------------+--------------------+

Methods
-------

+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                           | :ref:`_compute_cost<class_AStarGrid2D_method__compute_cost>` **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)** |virtual| |const|   |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`                           | :ref:`_estimate_cost<class_AStarGrid2D_method__estimate_cost>` **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)** |virtual| |const| |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                                | :ref:`clear<class_AStarGrid2D_method_clear>` **(** **)**                                                                                                                    |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PackedVector2Array<class_PackedVector2Array>` | :ref:`get_id_path<class_AStarGrid2D_method_get_id_path>` **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)**                         |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PackedVector2Array<class_PackedVector2Array>` | :ref:`get_point_path<class_AStarGrid2D_method_get_point_path>` **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)**                   |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                             | :ref:`is_dirty<class_AStarGrid2D_method_is_dirty>` **(** **)** |const|                                                                                                      |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                             | :ref:`is_in_bounds<class_AStarGrid2D_method_is_in_bounds>` **(** :ref:`int<class_int>` x, :ref:`int<class_int>` y **)** |const|                                             |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                             | :ref:`is_in_boundsv<class_AStarGrid2D_method_is_in_boundsv>` **(** :ref:`Vector2i<class_Vector2i>` id **)** |const|                                                         |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`                             | :ref:`is_point_solid<class_AStarGrid2D_method_is_point_solid>` **(** :ref:`Vector2i<class_Vector2i>` id **)** |const|                                                       |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                                | :ref:`set_point_solid<class_AStarGrid2D_method_set_point_solid>` **(** :ref:`Vector2i<class_Vector2i>` id, :ref:`bool<class_bool>` solid=true **)**                         |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                                | :ref:`update<class_AStarGrid2D_method_update>` **(** **)**                                                                                                                  |
+-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_AStarGrid2D_Heuristic:

.. _class_AStarGrid2D_constant_HEURISTIC_EUCLIDEAN:

.. _class_AStarGrid2D_constant_HEURISTIC_MANHATTAN:

.. _class_AStarGrid2D_constant_HEURISTIC_OCTILE:

.. _class_AStarGrid2D_constant_HEURISTIC_CHEBYSHEV:

.. _class_AStarGrid2D_constant_HEURISTIC_MAX:

enum **Heuristic**:

- **HEURISTIC_EUCLIDEAN** = **0**

- **HEURISTIC_MANHATTAN** = **1**

- **HEURISTIC_OCTILE** = **2**

- **HEURISTIC_CHEBYSHEV** = **3**

- **HEURISTIC_MAX** = **4**

----

.. _enum_AStarGrid2D_DiagonalMode:

.. _class_AStarGrid2D_constant_DIAGONAL_MODE_ALWAYS:

.. _class_AStarGrid2D_constant_DIAGONAL_MODE_NEVER:

.. _class_AStarGrid2D_constant_DIAGONAL_MODE_AT_LEAST_ONE_WALKABLE:

.. _class_AStarGrid2D_constant_DIAGONAL_MODE_ONLY_IF_NO_OBSTACLES:

.. _class_AStarGrid2D_constant_DIAGONAL_MODE_MAX:

enum **DiagonalMode**:

- **DIAGONAL_MODE_ALWAYS** = **0**

- **DIAGONAL_MODE_NEVER** = **1**

- **DIAGONAL_MODE_AT_LEAST_ONE_WALKABLE** = **2**

- **DIAGONAL_MODE_ONLY_IF_NO_OBSTACLES** = **3**

- **DIAGONAL_MODE_MAX** = **4**

Property Descriptions
---------------------

.. _class_AStarGrid2D_property_cell_size:

- :ref:`Vector2<class_Vector2>` **cell_size**

+-----------+----------------------+
| *Default* | ``Vector2(1, 1)``    |
+-----------+----------------------+
| *Setter*  | set_cell_size(value) |
+-----------+----------------------+
| *Getter*  | get_cell_size()      |
+-----------+----------------------+

----

.. _class_AStarGrid2D_property_default_heuristic:

- :ref:`Heuristic<enum_AStarGrid2D_Heuristic>` **default_heuristic**

+-----------+------------------------------+
| *Default* | ``0``                        |
+-----------+------------------------------+
| *Setter*  | set_default_heuristic(value) |
+-----------+------------------------------+
| *Getter*  | get_default_heuristic()      |
+-----------+------------------------------+

----

.. _class_AStarGrid2D_property_diagonal_mode:

- :ref:`DiagonalMode<enum_AStarGrid2D_DiagonalMode>` **diagonal_mode**

+-----------+--------------------------+
| *Default* | ``0``                    |
+-----------+--------------------------+
| *Setter*  | set_diagonal_mode(value) |
+-----------+--------------------------+
| *Getter*  | get_diagonal_mode()      |
+-----------+--------------------------+

----

.. _class_AStarGrid2D_property_jumping_enabled:

- :ref:`bool<class_bool>` **jumping_enabled**

+-----------+----------------------------+
| *Default* | ``false``                  |
+-----------+----------------------------+
| *Setter*  | set_jumping_enabled(value) |
+-----------+----------------------------+
| *Getter*  | is_jumping_enabled()       |
+-----------+----------------------------+

----

.. _class_AStarGrid2D_property_offset:

- :ref:`Vector2<class_Vector2>` **offset**

+-----------+-------------------+
| *Default* | ``Vector2(0, 0)`` |
+-----------+-------------------+
| *Setter*  | set_offset(value) |
+-----------+-------------------+
| *Getter*  | get_offset()      |
+-----------+-------------------+

----

.. _class_AStarGrid2D_property_size:

- :ref:`Vector2i<class_Vector2i>` **size**

+-----------+--------------------+
| *Default* | ``Vector2i(0, 0)`` |
+-----------+--------------------+
| *Setter*  | set_size(value)    |
+-----------+--------------------+
| *Getter*  | get_size()         |
+-----------+--------------------+

Method Descriptions
-------------------

.. _class_AStarGrid2D_method__compute_cost:

- :ref:`float<class_float>` **_compute_cost** **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)** |virtual| |const|

----

.. _class_AStarGrid2D_method__estimate_cost:

- :ref:`float<class_float>` **_estimate_cost** **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)** |virtual| |const|

----

.. _class_AStarGrid2D_method_clear:

- void **clear** **(** **)**

----

.. _class_AStarGrid2D_method_get_id_path:

- :ref:`PackedVector2Array<class_PackedVector2Array>` **get_id_path** **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)**

----

.. _class_AStarGrid2D_method_get_point_path:

- :ref:`PackedVector2Array<class_PackedVector2Array>` **get_point_path** **(** :ref:`Vector2i<class_Vector2i>` from_id, :ref:`Vector2i<class_Vector2i>` to_id **)**

----

.. _class_AStarGrid2D_method_is_dirty:

- :ref:`bool<class_bool>` **is_dirty** **(** **)** |const|

----

.. _class_AStarGrid2D_method_is_in_bounds:

- :ref:`bool<class_bool>` **is_in_bounds** **(** :ref:`int<class_int>` x, :ref:`int<class_int>` y **)** |const|

----

.. _class_AStarGrid2D_method_is_in_boundsv:

- :ref:`bool<class_bool>` **is_in_boundsv** **(** :ref:`Vector2i<class_Vector2i>` id **)** |const|

----

.. _class_AStarGrid2D_method_is_point_solid:

- :ref:`bool<class_bool>` **is_point_solid** **(** :ref:`Vector2i<class_Vector2i>` id **)** |const|

----

.. _class_AStarGrid2D_method_set_point_solid:

- void **set_point_solid** **(** :ref:`Vector2i<class_Vector2i>` id, :ref:`bool<class_bool>` solid=true **)**

----

.. _class_AStarGrid2D_method_update:

- void **update** **(** **)**

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
