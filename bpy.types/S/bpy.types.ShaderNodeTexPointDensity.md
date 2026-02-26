# ShaderNodeTexPointDensity(ShaderNode)

base classes — [[bpy_struct]], [[Node]], [[NodeInternal]], [[ShaderNode]]

_class _bpy.types.ShaderNodeTexPointDensity(_ShaderNode_)
    

Generate a volumetric point for each particle or vertex of another object

interpolation
    

Texture interpolation

  * `Closest` Closest – No interpolation (sample closest texel).

  * `Linear` Linear – Linear interpolation.

  * `Cubic` Cubic – Cubic interpolation.


Type:
    

enum in [`'Closest'`, `'Linear'`, `'Cubic'`], default `'Linear'`

object
    

Object to take point data from

Type:
    

[[Object]]

particle_color_source
    

Data to derive color results from

  * `PARTICLE_AGE` Particle Age – Lifetime mapped as 0.0 to 1.0 intensity.

  * `PARTICLE_SPEED` Particle Speed – Particle speed (absolute magnitude of velocity) mapped as 0.0 to 1.0 intensity.

  * `PARTICLE_VELOCITY` Particle Velocity – XYZ velocity mapped to RGB colors.


Type:
    

enum in [`'PARTICLE_AGE'`, `'PARTICLE_SPEED'`, `'PARTICLE_VELOCITY'`], default `'PARTICLE_AGE'`

particle_system
    

Particle System to render as points

Type:
    

[[ParticleSystem]]

point_source
    

Point data to use as renderable point density

  * `PARTICLE_SYSTEM` Particle System – Generate point density from a particle system.

  * `OBJECT` Object Vertices – Generate point density from an object’s vertices.


Type:
    

enum in [`'PARTICLE_SYSTEM'`, `'OBJECT'`], default `'PARTICLE_SYSTEM'`

radius
    

Radius from the shaded sample to look for points within

Type:
    

float in [0.001, inf], default 0.0

resolution
    

Resolution used by the texture holding the point density

Type:
    

int in [1, 32768], default 0

space
    

Coordinate system to calculate voxels in

Type:
    

enum in [`'OBJECT'`, `'WORLD'`], default `'OBJECT'`

vertex_attribute_name
    

Vertex attribute to use for color

Type:
    

string, default “”, (never None)

vertex_color_source
    

Data to derive color results from

  * `VERTEX_COLOR` Vertex Color – Vertex color layer.

  * `VERTEX_WEIGHT` Vertex Weight – Vertex group weight.

  * `VERTEX_NORMAL` Vertex Normal – XYZ normal vector mapped to RGB colors.


Type:
    

enum in [`'VERTEX_COLOR'`, `'VERTEX_WEIGHT'`, `'VERTEX_NORMAL'`], default `'VERTEX_COLOR'`

_classmethod _is_registered_node_type()
    

True if a registered node type

Returns:
    

Result

Return type:
    

boolean

_classmethod _input_template(_index_)
    

Input socket template

Parameters:
    

**index** (_int in_ _[__0_ _,__inf_ _]_) – Index

Returns:
    

result

Return type:
    

[[NodeInternalSocketTemplate]]

_classmethod _output_template(_index_)
    

Output socket template

Parameters:
    

**index** (_int in_ _[__0_ _,__inf_ _]_) – Index

Returns:
    

result

Return type:
    

[[NodeInternalSocketTemplate]]

cache_point_density(_*_ , _depsgraph =None_)
    

Cache point density data for later calculation

calc_point_density(_*_ , _depsgraph =None_)
    

Calculate point density

Returns:
    

RGBA Values

Return type:
    

float array of 1 items in [-inf, inf]

calc_point_density_minmax(_*_ , _depsgraph =None_)
    

Calculate point density

Returns:
    

min, min, [[mathutils.Vector]] of 3 items in [-inf, inf]

max, max, [[mathutils.Vector]] of 3 items in [-inf, inf]

Return type:
    

([[mathutils.Vector]] of 3 items in [-inf, inf], [[mathutils.Vector]] of 3 items in [-inf, inf])

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[[bpy.types.Struct]] subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [[bpy_struct.id_data]]
  * [[Node.type]]
  * [[Node.location]]
  * [[Node.location_absolute]]
  * [[Node.width]]
  * [[Node.height]]
  * [[Node.dimensions]]
  * [[Node.name]]
  * [[Node.label]]
  * [[Node.inputs]]
  * [[Node.outputs]]
  * [[Node.internal_links]]
  * [[Node.parent]]
  * [[Node.warning_propagation]]
  * [[Node.use_custom_color]]
  * [[Node.color]]
  * [[Node.color_tag]]

| 

  * [[Node.select]]
  * [[Node.show_options]]
  * [[Node.show_preview]]
  * [[Node.hide]]
  * [[Node.mute]]
  * [[Node.show_texture]]
  * [[Node.bl_idname]]
  * [[Node.bl_label]]
  * [[Node.bl_description]]
  * [[Node.bl_icon]]
  * [[Node.bl_static_type]]
  * [[Node.bl_width_default]]
  * [[Node.bl_width_min]]
  * [[Node.bl_width_max]]
  * [[Node.bl_height_default]]
  * [[Node.bl_height_min]]
  * [[Node.bl_height_max]]

  
---|---  
  
## Inherited Functions

  * [[bpy_struct.as_pointer]]
  * [[bpy_struct.driver_add]]
  * [[bpy_struct.driver_remove]]
  * [[bpy_struct.get]]
  * [[bpy_struct.id_properties_clear]]
  * [[bpy_struct.id_properties_ensure]]
  * [[bpy_struct.id_properties_ui]]
  * [[bpy_struct.is_property_hidden]]
  * [[bpy_struct.is_property_overridable_library]]
  * [[bpy_struct.is_property_readonly]]
  * [[bpy_struct.is_property_set]]
  * [[bpy_struct.items]]
  * [[bpy_struct.keyframe_delete]]
  * [[bpy_struct.keyframe_insert]]
  * [[bpy_struct.keys]]
  * [[bpy_struct.path_from_id]]
  * [[bpy_struct.path_resolve]]
  * [[bpy_struct.pop]]
  * [[bpy_struct.property_overridable_library_set]]
  * [[bpy_struct.property_unset]]
  * [[bpy_struct.rna_ancestors]]
  * [[bpy_struct.type_recast]]
  * [[bpy_struct.values]]
  * [[Node.socket_value_update]]
  * [[Node.is_registered_node_type]]

| 

  * [[Node.poll]]
  * [[Node.poll_instance]]
  * [[Node.update]]
  * [[Node.insert_link]]
  * [[Node.init]]
  * [[Node.copy]]
  * [[Node.free]]
  * [[Node.draw_buttons]]
  * [[Node.draw_buttons_ext]]
  * [[Node.draw_label]]
  * [[Node.debug_zone_body_lazy_function_graph]]
  * [[Node.debug_zone_lazy_function_graph]]
  * [[Node.poll]]
  * [[Node.bl_rna_get_subclass]]
  * [[Node.bl_rna_get_subclass_py]]
  * [[NodeInternal.poll]]
  * [[NodeInternal.poll_instance]]
  * [[NodeInternal.update]]
  * [[NodeInternal.draw_buttons]]
  * [[NodeInternal.draw_buttons_ext]]
  * [[NodeInternal.bl_rna_get_subclass]]
  * [[NodeInternal.bl_rna_get_subclass_py]]
  * `ShaderNode.poll`
  * [[ShaderNode.bl_rna_get_subclass]]
  * [[ShaderNode.bl_rna_get_subclass_py]]

  
---|---
