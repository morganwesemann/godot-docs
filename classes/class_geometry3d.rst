:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/Geometry3D.xml.

.. _class_Geometry3D:

Geometry3D
==========

**Inherits:** :ref:`Object<class_Object>`

Provides methods for some common 3D geometric operations.

.. rst-class:: classref-introduction-group

Description
-----------

Provides a set of helper functions to create geometric shapes, compute intersections between shapes, and process various other geometric operations in 3D.

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Plane[]<class_Plane>`                         | :ref:`build_box_planes<class_Geometry3D_method_build_box_planes>` **(** :ref:`Vector3<class_Vector3>` extents **)**                                                                                                                                                         |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Plane[]<class_Plane>`                         | :ref:`build_capsule_planes<class_Geometry3D_method_build_capsule_planes>` **(** :ref:`float<class_float>` radius, :ref:`float<class_float>` height, :ref:`int<class_int>` sides, :ref:`int<class_int>` lats, Vector3.Axis axis=2 **)**                                      |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Plane[]<class_Plane>`                         | :ref:`build_cylinder_planes<class_Geometry3D_method_build_cylinder_planes>` **(** :ref:`float<class_float>` radius, :ref:`float<class_float>` height, :ref:`int<class_int>` sides, Vector3.Axis axis=2 **)**                                                                |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`clip_polygon<class_Geometry3D_method_clip_polygon>` **(** :ref:`PackedVector3Array<class_PackedVector3Array>` points, :ref:`Plane<class_Plane>` plane **)**                                                                                                           |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`compute_convex_mesh_points<class_Geometry3D_method_compute_convex_mesh_points>` **(** :ref:`Plane[]<class_Plane>` planes **)**                                                                                                                                        |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                       | :ref:`get_closest_point_to_segment<class_Geometry3D_method_get_closest_point_to_segment>` **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` s1, :ref:`Vector3<class_Vector3>` s2 **)**                                                               |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                       | :ref:`get_closest_point_to_segment_uncapped<class_Geometry3D_method_get_closest_point_to_segment_uncapped>` **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` s1, :ref:`Vector3<class_Vector3>` s2 **)**                                             |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`get_closest_points_between_segments<class_Geometry3D_method_get_closest_points_between_segments>` **(** :ref:`Vector3<class_Vector3>` p1, :ref:`Vector3<class_Vector3>` p2, :ref:`Vector3<class_Vector3>` q1, :ref:`Vector3<class_Vector3>` q2 **)**                  |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                       | :ref:`get_triangle_barycentric_coords<class_Geometry3D_method_get_triangle_barycentric_coords>` **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)**                          |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Variant<class_Variant>`                       | :ref:`ray_intersects_triangle<class_Geometry3D_method_ray_intersects_triangle>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` dir, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)**        |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`segment_intersects_convex<class_Geometry3D_method_segment_intersects_convex>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Plane[]<class_Plane>` planes **)**                                                                    |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`segment_intersects_cylinder<class_Geometry3D_method_segment_intersects_cylinder>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` height, :ref:`float<class_float>` radius **)**                                |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`segment_intersects_sphere<class_Geometry3D_method_segment_intersects_sphere>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` sphere_position, :ref:`float<class_float>` sphere_radius **)**                |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Variant<class_Variant>`                       | :ref:`segment_intersects_triangle<class_Geometry3D_method_segment_intersects_triangle>` **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)** |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedInt32Array<class_PackedInt32Array>`     | :ref:`tetrahedralize_delaunay<class_Geometry3D_method_tetrahedralize_delaunay>` **(** :ref:`PackedVector3Array<class_PackedVector3Array>` points **)**                                                                                                                      |
   +-----------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_Geometry3D_method_build_box_planes:

.. rst-class:: classref-method

:ref:`Plane[]<class_Plane>` **build_box_planes** **(** :ref:`Vector3<class_Vector3>` extents **)**

Returns an array with 6 :ref:`Plane<class_Plane>`\ s that describe the sides of a box centered at the origin. The box size is defined by ``extents``, which represents one (positive) corner of the box (i.e. half its actual size).

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_build_capsule_planes:

.. rst-class:: classref-method

:ref:`Plane[]<class_Plane>` **build_capsule_planes** **(** :ref:`float<class_float>` radius, :ref:`float<class_float>` height, :ref:`int<class_int>` sides, :ref:`int<class_int>` lats, Vector3.Axis axis=2 **)**

Returns an array of :ref:`Plane<class_Plane>`\ s closely bounding a faceted capsule centered at the origin with radius ``radius`` and height ``height``. The parameter ``sides`` defines how many planes will be generated for the side part of the capsule, whereas ``lats`` gives the number of latitudinal steps at the bottom and top of the capsule. The parameter ``axis`` describes the axis along which the capsule is oriented (0 for X, 1 for Y, 2 for Z).

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_build_cylinder_planes:

.. rst-class:: classref-method

:ref:`Plane[]<class_Plane>` **build_cylinder_planes** **(** :ref:`float<class_float>` radius, :ref:`float<class_float>` height, :ref:`int<class_int>` sides, Vector3.Axis axis=2 **)**

Returns an array of :ref:`Plane<class_Plane>`\ s closely bounding a faceted cylinder centered at the origin with radius ``radius`` and height ``height``. The parameter ``sides`` defines how many planes will be generated for the round part of the cylinder. The parameter ``axis`` describes the axis along which the cylinder is oriented (0 for X, 1 for Y, 2 for Z).

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_clip_polygon:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **clip_polygon** **(** :ref:`PackedVector3Array<class_PackedVector3Array>` points, :ref:`Plane<class_Plane>` plane **)**

Clips the polygon defined by the points in ``points`` against the ``plane`` and returns the points of the clipped polygon.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_compute_convex_mesh_points:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **compute_convex_mesh_points** **(** :ref:`Plane[]<class_Plane>` planes **)**

Calculates and returns all the vertex points of a convex shape defined by an array of ``planes``.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_get_closest_point_to_segment:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_closest_point_to_segment** **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` s1, :ref:`Vector3<class_Vector3>` s2 **)**

Returns the 3D point on the 3D segment (``s1``, ``s2``) that is closest to ``point``. The returned point will always be inside the specified segment.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_get_closest_point_to_segment_uncapped:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_closest_point_to_segment_uncapped** **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` s1, :ref:`Vector3<class_Vector3>` s2 **)**

Returns the 3D point on the 3D line defined by (``s1``, ``s2``) that is closest to ``point``. The returned point can be inside the segment (``s1``, ``s2``) or outside of it, i.e. somewhere on the line extending from the segment.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_get_closest_points_between_segments:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **get_closest_points_between_segments** **(** :ref:`Vector3<class_Vector3>` p1, :ref:`Vector3<class_Vector3>` p2, :ref:`Vector3<class_Vector3>` q1, :ref:`Vector3<class_Vector3>` q2 **)**

Given the two 3D segments (``p1``, ``p2``) and (``q1``, ``q2``), finds those two points on the two segments that are closest to each other. Returns a :ref:`PackedVector3Array<class_PackedVector3Array>` that contains this point on (``p1``, ``p2``) as well the accompanying point on (``q1``, ``q2``).

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_get_triangle_barycentric_coords:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_triangle_barycentric_coords** **(** :ref:`Vector3<class_Vector3>` point, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)**

Returns a :ref:`Vector3<class_Vector3>` containing weights based on how close a 3D position (``point``) is to a triangle's different vertices (``a``, ``b`` and ``c``). This is useful for interpolating between the data of different vertices in a triangle. One example use case is using this to smoothly rotate over a mesh instead of relying solely on face normals.

\ `Here is a more detailed explanation of barycentric coordinates. <https://en.wikipedia.org/wiki/Barycentric_coordinate_system>`__

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_ray_intersects_triangle:

.. rst-class:: classref-method

:ref:`Variant<class_Variant>` **ray_intersects_triangle** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` dir, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)**

Tests if the 3D ray starting at ``from`` with the direction of ``dir`` intersects the triangle specified by ``a``, ``b`` and ``c``. If yes, returns the point of intersection as :ref:`Vector3<class_Vector3>`. If no intersection takes place, returns ``null``.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_segment_intersects_convex:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **segment_intersects_convex** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Plane[]<class_Plane>` planes **)**

Given a convex hull defined though the :ref:`Plane<class_Plane>`\ s in the array ``planes``, tests if the segment (``from``, ``to``) intersects with that hull. If an intersection is found, returns a :ref:`PackedVector3Array<class_PackedVector3Array>` containing the point the intersection and the hull's normal. Otherwise, returns an empty array.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_segment_intersects_cylinder:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **segment_intersects_cylinder** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`float<class_float>` height, :ref:`float<class_float>` radius **)**

Checks if the segment (``from``, ``to``) intersects the cylinder with height ``height`` that is centered at the origin and has radius ``radius``. If no, returns an empty :ref:`PackedVector3Array<class_PackedVector3Array>`. If an intersection takes place, the returned array contains the point of intersection and the cylinder's normal at the point of intersection.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_segment_intersects_sphere:

.. rst-class:: classref-method

:ref:`PackedVector3Array<class_PackedVector3Array>` **segment_intersects_sphere** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` sphere_position, :ref:`float<class_float>` sphere_radius **)**

Checks if the segment (``from``, ``to``) intersects the sphere that is located at ``sphere_position`` and has radius ``sphere_radius``. If no, returns an empty :ref:`PackedVector3Array<class_PackedVector3Array>`. If yes, returns a :ref:`PackedVector3Array<class_PackedVector3Array>` containing the point of intersection and the sphere's normal at the point of intersection.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_segment_intersects_triangle:

.. rst-class:: classref-method

:ref:`Variant<class_Variant>` **segment_intersects_triangle** **(** :ref:`Vector3<class_Vector3>` from, :ref:`Vector3<class_Vector3>` to, :ref:`Vector3<class_Vector3>` a, :ref:`Vector3<class_Vector3>` b, :ref:`Vector3<class_Vector3>` c **)**

Tests if the segment (``from``, ``to``) intersects the triangle ``a``, ``b``, ``c``. If yes, returns the point of intersection as :ref:`Vector3<class_Vector3>`. If no intersection takes place, returns ``null``.

.. rst-class:: classref-item-separator

----

.. _class_Geometry3D_method_tetrahedralize_delaunay:

.. rst-class:: classref-method

:ref:`PackedInt32Array<class_PackedInt32Array>` **tetrahedralize_delaunay** **(** :ref:`PackedVector3Array<class_PackedVector3Array>` points **)**

Tetrahedralizes the volume specified by a discrete set of ``points`` in 3D space, ensuring that no point lies within the circumsphere of any resulting tetrahedron. The method returns a :ref:`PackedInt32Array<class_PackedInt32Array>` where each tetrahedron consists of four consecutive point indices into the ``points`` array (resulting in an array with ``n * 4`` elements, where ``n`` is the number of tetrahedra found). If the tetrahedralization is unsuccessful, an empty :ref:`PackedInt32Array<class_PackedInt32Array>` is returned.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
