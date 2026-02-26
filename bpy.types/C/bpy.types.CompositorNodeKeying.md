# CompositorNodeKeying(CompositorNode)

base classes — [[bpy_struct]], [[Node]], [[NodeInternal]], [[CompositorNode]]

_class _bpy.types.CompositorNodeKeying(_CompositorNode_)
    

Perform both chroma keying (to remove the backdrop) and despill (to correct color cast from the backdrop)

blur_post
    

Matte blur size which applies after clipping and dilate/eroding. (Deprecated: Use Postprocess Blur Size input instead.)

Type:
    

int in [0, 2048], default 0

blur_pre
    

Chroma pre-blur size which applies before running keyer. (Deprecated: Use Preprocess Blur Size input instead.)

Type:
    

int in [0, 2048], default 0

clip_black
    

Value of non-scaled matte pixel which considers as fully background pixel. (Deprecated: Use Black Level input instead.)

Type:
    

float in [0, 1], default 0.0

clip_white
    

Value of non-scaled matte pixel which considers as fully foreground pixel. (Deprecated: Use White Level input instead.)

Type:
    

float in [0, 1], default 0.0

despill_balance
    

Balance between non-key colors used to detect amount of key color to be removed. (Deprecated: Use Despill Balance input instead.)

Type:
    

float in [0, 1], default 0.0

despill_factor
    

Factor of despilling screen color from image. (Deprecated: Use Despill Strength input instead.)

Type:
    

float in [0, 1], default 0.0

dilate_distance
    

Distance to grow/shrink the matte. (Deprecated: Use Postprocess Dilate Size input instead.)

Type:
    

int in [-100, 100], default 0

edge_kernel_radius
    

Radius of kernel used to detect whether pixel belongs to edge. (Deprecated: Use Edge Search Size input instead.)

Type:
    

int in [0, 100], default 0

edge_kernel_tolerance
    

Tolerance to pixels inside kernel which are treating as belonging to the same plane. (Deprecated: Use Edge Tolerance input instead.)

Type:
    

float in [0, 1], default 0.0

feather_distance
    

Distance to grow/shrink the feather. (Deprecated: Use Postprocess Feather Size input instead.)

Type:
    

int in [-100, 100], default 0

feather_falloff
    

Falloff type of the feather

Type:
    

enum in [Proportional Falloff Curve Only Items](bpy_types_enum_items/proportional_falloff_curve_only_items.md#rna-enum-proportional-falloff-curve-only-items), default `'SMOOTH'`

screen_balance
    

Balance between two non-primary channels primary channel is comparing against. (Deprecated: Use Key Balance input instead.)

Type:
    

float in [0, 1], default 0.0

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
