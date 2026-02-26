# CompositorNodeTonemap(CompositorNode)

base classes — [[bpy_struct]], [[Node]], [[NodeInternal]], [[CompositorNode]]

_class _bpy.types.CompositorNodeTonemap(_CompositorNode_)
    

Map one set of colors to another in order to approximate the appearance of high dynamic range

adaptation
    

If 0, global; if 1, based on pixel intensity. (Deprecated: Use Light Adaptation input instead.)

Type:
    

float in [0, 1], default 0.0

contrast
    

Set to 0 to use estimate from input image. (Deprecated: Use Contrast input instead.)

Type:
    

float in [0, 1], default 0.0

correction
    

If 0, same for all channels; if 1, each independent (Deprecated: Use Chromatic Adaptation input instead.)

Type:
    

float in [0, 1], default 0.0

gamma
    

If not used, set to 1. (Deprecated: Use Gamma input instead.)

Type:
    

float in [0.001, 3], default 0.0

intensity
    

If less than zero, darkens image; otherwise, makes it brighter. (Deprecated: Use Intensity input instead.)

Type:
    

float in [-8, 8], default 0.0

key
    

The value the average luminance is mapped to. (Deprecated: Use Key input instead.)

Type:
    

float in [0, 1], default 0.0

offset
    

Normally always 1, but can be used as an extra control to alter the brightness curve. (Deprecated: Use Balance input instead.)

Type:
    

float in [0.001, 10], default 0.0

tonemap_type
    

  * `RD_PHOTORECEPTOR` R/D Photoreceptor – More advanced algorithm based on eye physiology, by Reinhard and Devlin.

  * `RH_SIMPLE` Rh Simple – Simpler photographic algorithm by Reinhard.


Type:
    

enum in [`'RD_PHOTORECEPTOR'`, `'RH_SIMPLE'`], default `'RH_SIMPLE'`

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
