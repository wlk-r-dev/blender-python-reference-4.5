# CompositorNodeColorBalance(CompositorNode)

base classes — [[bpy_struct]], [[Node]], [[NodeInternal]], [[CompositorNode]]

_class _bpy.types.CompositorNodeColorBalance(_CompositorNode_)
    

Adjust color and values

correction_method
    

  * `LIFT_GAMMA_GAIN` Lift/Gamma/Gain.

  * `OFFSET_POWER_SLOPE` Offset/Power/Slope (ASC-CDL) – ASC-CDL standard color correction.

  * `WHITEPOINT` White Point – Chromatic adaption from a different white point.


Type:
    

enum in [`'LIFT_GAMMA_GAIN'`, `'OFFSET_POWER_SLOPE'`, `'WHITEPOINT'`], default `'LIFT_GAMMA_GAIN'`

gain
    

Correction for highlights. (Deprecated: Use Gain input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (1.0, 1.0, 1.0)

gamma
    

Correction for midtones. (Deprecated: Use Gamma input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (1.0, 1.0, 1.0)

input_temperature
    

Color temperature of the input’s white point. (Deprecated: Use Input Temperature input instead.)

Type:
    

float in [1800, 100000], default 6500.0

input_tint
    

Color tint of the input’s white point (the default of 10 matches daylight). (Deprecated: Use Input Tint input instead.)

Type:
    

float in [-500, 500], default 10.0

input_whitepoint
    

The color which gets mapped to white (automatically converted to/from temperature and tint)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (0.0, 0.0, 0.0)

lift
    

Correction for shadows. (Deprecated: Use Lift input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (1.0, 1.0, 1.0)

offset
    

Correction for entire tonal range. (Deprecated: Use Offset input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (0.0, 0.0, 0.0)

offset_basis
    

Support negative color by using this as the RGB basis. (Deprecated: Use Offset Basis input instead.)

Type:
    

float in [-inf, inf], default 0.0

output_temperature
    

Color temperature of the output’s white point. (Deprecated: Use Output Temperature input instead.)

Type:
    

float in [1800, 100000], default 6500.0

output_tint
    

Color tint of the output’s white point (the default of 10 matches daylight). (Deprecated: Use Output Tint input instead.)

Type:
    

float in [-500, 500], default 10.0

output_whitepoint
    

The color which gets white gets mapped to (automatically converted to/from temperature and tint)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (0.0, 0.0, 0.0)

power
    

Correction for midtones. (Deprecated: Use Power input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (1.0, 1.0, 1.0)

slope
    

Correction for highlights. (Deprecated: Use Slope input instead.)

Type:
    

[[mathutils.Color]] of 3 items in [0, inf], default (1.0, 1.0, 1.0)

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

update()
    

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
  * [[Node.poll]]

| 

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
  * [[CompositorNode.tag_need_exec]]
  * `CompositorNode.poll`
  * [[CompositorNode.update]]
  * [[CompositorNode.bl_rna_get_subclass]]
  * [[CompositorNode.bl_rna_get_subclass_py]]

  
---|---
