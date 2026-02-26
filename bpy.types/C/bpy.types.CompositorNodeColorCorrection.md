# CompositorNodeColorCorrection(CompositorNode)

base classes — [[bpy_struct]], [[Node]], [[NodeInternal]], [[CompositorNode]]

_class _bpy.types.CompositorNodeColorCorrection(_CompositorNode_)
    

Adjust the color of an image, separately in several tonal ranges (highlights, midtones and shadows)

blue
    

Blue channel active. (Deprecated: Use Apply On Blue input instead.)

Type:
    

boolean, default True

green
    

Green channel active. (Deprecated: Use Apply On Green input instead.)

Type:
    

boolean, default True

highlights_contrast
    

Highlights contrast. (Deprecated: Use Highlights Contrast input instead.)

Type:
    

float in [0, 4], default 1.0

highlights_gain
    

Highlights gain. (Deprecated: Use Highlights Gain input instead.)

Type:
    

float in [0, 4], default 1.0

highlights_gamma
    

Highlights gamma. (Deprecated: Use Highlights Gamma input instead.)

Type:
    

float in [0, 4], default 1.0

highlights_lift
    

Highlights lift. (Deprecated: Use Highlights Lift input instead.)

Type:
    

float in [-1, 1], default 0.0

highlights_saturation
    

Highlights saturation. (Deprecated: Use Highlights Saturation input instead.)

Type:
    

float in [0, 4], default 1.0

master_contrast
    

Master contrast. (Deprecated: Use Master Contrast input instead.)

Type:
    

float in [0, 4], default 1.0

master_gain
    

Master gain. (Deprecated: Use Master Gain input instead.)

Type:
    

float in [0, 4], default 1.0

master_gamma
    

Master gamma. (Deprecated: Use Master Gamma input instead.)

Type:
    

float in [0, 4], default 1.0

master_lift
    

Master lift. (Deprecated: Use Master Lift input instead.)

Type:
    

float in [-1, 1], default 0.0

master_saturation
    

Master saturation. (Deprecated: Use Master Saturation input instead.)

Type:
    

float in [0, 4], default 1.0

midtones_contrast
    

Midtones contrast. (Deprecated: Use Midtones Contrast input instead.)

Type:
    

float in [0, 4], default 1.0

midtones_end
    

End of midtones. (Deprecated: Use Midtones End input instead.)

Type:
    

float in [0, 1], default 0.7

midtones_gain
    

Midtones gain. (Deprecated: Use Midtones Gain input instead.)

Type:
    

float in [0, 4], default 1.0

midtones_gamma
    

Midtones gamma. (Deprecated: Use Midtones Gamma input instead.)

Type:
    

float in [0, 4], default 1.0

midtones_lift
    

Midtones lift. (Deprecated: Use Midtones Lift input instead.)

Type:
    

float in [-1, 1], default 0.0

midtones_saturation
    

Midtones saturation. (Deprecated: Use Midtones Saturation input instead.)

Type:
    

float in [0, 4], default 1.0

midtones_start
    

Start of midtones. (Deprecated: Use Midtones Start input instead.)

Type:
    

float in [0, 1], default 0.2

red
    

Red channel active. (Deprecated: Use Apply On Red input instead.)

Type:
    

boolean, default True

shadows_contrast
    

Shadows contrast. (Deprecated: Use Shadows Contrast input instead.)

Type:
    

float in [0, 4], default 1.0

shadows_gain
    

Shadows gain. (Deprecated: Use Shadows Gain input instead.)

Type:
    

float in [0, 4], default 1.0

shadows_gamma
    

Shadows gamma. (Deprecated: Use Shadows Gamma input instead.)

Type:
    

float in [0, 4], default 1.0

shadows_lift
    

Shadows lift. (Deprecated: Use Shadows Lift input instead.)

Type:
    

float in [-1, 1], default 0.0

shadows_saturation
    

Shadows saturation. (Deprecated: Use Shadows Saturation input instead.)

Type:
    

float in [0, 4], default 1.0

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
