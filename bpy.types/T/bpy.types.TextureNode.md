# TextureNode(NodeInternal)

base classes — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`Node`](bpy.types.Node.html#bpy.types.Node "bpy.types.Node"), [`NodeInternal`](bpy.types.NodeInternal.html#bpy.types.NodeInternal "bpy.types.NodeInternal")

subclasses — [`TextureNodeAt`](bpy.types.TextureNodeAt.html#bpy.types.TextureNodeAt "bpy.types.TextureNodeAt"), [`TextureNodeBricks`](bpy.types.TextureNodeBricks.html#bpy.types.TextureNodeBricks "bpy.types.TextureNodeBricks"), [`TextureNodeChecker`](bpy.types.TextureNodeChecker.html#bpy.types.TextureNodeChecker "bpy.types.TextureNodeChecker"), [`TextureNodeCombineColor`](bpy.types.TextureNodeCombineColor.html#bpy.types.TextureNodeCombineColor "bpy.types.TextureNodeCombineColor"), [`TextureNodeCompose`](bpy.types.TextureNodeCompose.html#bpy.types.TextureNodeCompose "bpy.types.TextureNodeCompose"), [`TextureNodeCoordinates`](bpy.types.TextureNodeCoordinates.html#bpy.types.TextureNodeCoordinates "bpy.types.TextureNodeCoordinates"), [`TextureNodeCurveRGB`](bpy.types.TextureNodeCurveRGB.html#bpy.types.TextureNodeCurveRGB "bpy.types.TextureNodeCurveRGB"), [`TextureNodeCurveTime`](bpy.types.TextureNodeCurveTime.html#bpy.types.TextureNodeCurveTime "bpy.types.TextureNodeCurveTime"), [`TextureNodeDecompose`](bpy.types.TextureNodeDecompose.html#bpy.types.TextureNodeDecompose "bpy.types.TextureNodeDecompose"), [`TextureNodeDistance`](bpy.types.TextureNodeDistance.html#bpy.types.TextureNodeDistance "bpy.types.TextureNodeDistance"), [`TextureNodeGroup`](bpy.types.TextureNodeGroup.html#bpy.types.TextureNodeGroup "bpy.types.TextureNodeGroup"), [`TextureNodeHueSaturation`](bpy.types.TextureNodeHueSaturation.html#bpy.types.TextureNodeHueSaturation "bpy.types.TextureNodeHueSaturation"), [`TextureNodeImage`](bpy.types.TextureNodeImage.html#bpy.types.TextureNodeImage "bpy.types.TextureNodeImage"), [`TextureNodeInvert`](bpy.types.TextureNodeInvert.html#bpy.types.TextureNodeInvert "bpy.types.TextureNodeInvert"), [`TextureNodeMath`](bpy.types.TextureNodeMath.html#bpy.types.TextureNodeMath "bpy.types.TextureNodeMath"), [`TextureNodeMixRGB`](bpy.types.TextureNodeMixRGB.html#bpy.types.TextureNodeMixRGB "bpy.types.TextureNodeMixRGB"), [`TextureNodeOutput`](bpy.types.TextureNodeOutput.html#bpy.types.TextureNodeOutput "bpy.types.TextureNodeOutput"), [`TextureNodeRGBToBW`](bpy.types.TextureNodeRGBToBW.html#bpy.types.TextureNodeRGBToBW "bpy.types.TextureNodeRGBToBW"), [`TextureNodeRotate`](bpy.types.TextureNodeRotate.html#bpy.types.TextureNodeRotate "bpy.types.TextureNodeRotate"), [`TextureNodeScale`](bpy.types.TextureNodeScale.html#bpy.types.TextureNodeScale "bpy.types.TextureNodeScale"), [`TextureNodeSeparateColor`](bpy.types.TextureNodeSeparateColor.html#bpy.types.TextureNodeSeparateColor "bpy.types.TextureNodeSeparateColor"), [`TextureNodeTexBlend`](bpy.types.TextureNodeTexBlend.html#bpy.types.TextureNodeTexBlend "bpy.types.TextureNodeTexBlend"), [`TextureNodeTexClouds`](bpy.types.TextureNodeTexClouds.html#bpy.types.TextureNodeTexClouds "bpy.types.TextureNodeTexClouds"), [`TextureNodeTexDistNoise`](bpy.types.TextureNodeTexDistNoise.html#bpy.types.TextureNodeTexDistNoise "bpy.types.TextureNodeTexDistNoise"), [`TextureNodeTexMagic`](bpy.types.TextureNodeTexMagic.html#bpy.types.TextureNodeTexMagic "bpy.types.TextureNodeTexMagic"), [`TextureNodeTexMarble`](bpy.types.TextureNodeTexMarble.html#bpy.types.TextureNodeTexMarble "bpy.types.TextureNodeTexMarble"), [`TextureNodeTexMusgrave`](bpy.types.TextureNodeTexMusgrave.html#bpy.types.TextureNodeTexMusgrave "bpy.types.TextureNodeTexMusgrave"), [`TextureNodeTexNoise`](bpy.types.TextureNodeTexNoise.html#bpy.types.TextureNodeTexNoise "bpy.types.TextureNodeTexNoise"), [`TextureNodeTexStucci`](bpy.types.TextureNodeTexStucci.html#bpy.types.TextureNodeTexStucci "bpy.types.TextureNodeTexStucci"), [`TextureNodeTexVoronoi`](bpy.types.TextureNodeTexVoronoi.html#bpy.types.TextureNodeTexVoronoi "bpy.types.TextureNodeTexVoronoi"), [`TextureNodeTexWood`](bpy.types.TextureNodeTexWood.html#bpy.types.TextureNodeTexWood "bpy.types.TextureNodeTexWood"), [`TextureNodeTexture`](bpy.types.TextureNodeTexture.html#bpy.types.TextureNodeTexture "bpy.types.TextureNodeTexture"), [`TextureNodeTranslate`](bpy.types.TextureNodeTranslate.html#bpy.types.TextureNodeTranslate "bpy.types.TextureNodeTranslate"), [`TextureNodeValToNor`](bpy.types.TextureNodeValToNor.html#bpy.types.TextureNodeValToNor "bpy.types.TextureNodeValToNor"), [`TextureNodeValToRGB`](bpy.types.TextureNodeValToRGB.html#bpy.types.TextureNodeValToRGB "bpy.types.TextureNodeValToRGB"), [`TextureNodeViewer`](bpy.types.TextureNodeViewer.html#bpy.types.TextureNodeViewer "bpy.types.TextureNodeViewer")

_class _bpy.types.TextureNode(_NodeInternal_)
    

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.html#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")
  * [`Node.type`](bpy.types.Node.html#bpy.types.Node.type "bpy.types.Node.type")
  * [`Node.location`](bpy.types.Node.html#bpy.types.Node.location "bpy.types.Node.location")
  * [`Node.location_absolute`](bpy.types.Node.html#bpy.types.Node.location_absolute "bpy.types.Node.location_absolute")
  * [`Node.width`](bpy.types.Node.html#bpy.types.Node.width "bpy.types.Node.width")
  * [`Node.height`](bpy.types.Node.html#bpy.types.Node.height "bpy.types.Node.height")
  * [`Node.dimensions`](bpy.types.Node.html#bpy.types.Node.dimensions "bpy.types.Node.dimensions")
  * [`Node.name`](bpy.types.Node.html#bpy.types.Node.name "bpy.types.Node.name")
  * [`Node.label`](bpy.types.Node.html#bpy.types.Node.label "bpy.types.Node.label")
  * [`Node.inputs`](bpy.types.Node.html#bpy.types.Node.inputs "bpy.types.Node.inputs")
  * [`Node.outputs`](bpy.types.Node.html#bpy.types.Node.outputs "bpy.types.Node.outputs")
  * [`Node.internal_links`](bpy.types.Node.html#bpy.types.Node.internal_links "bpy.types.Node.internal_links")
  * [`Node.parent`](bpy.types.Node.html#bpy.types.Node.parent "bpy.types.Node.parent")
  * [`Node.warning_propagation`](bpy.types.Node.html#bpy.types.Node.warning_propagation "bpy.types.Node.warning_propagation")
  * [`Node.use_custom_color`](bpy.types.Node.html#bpy.types.Node.use_custom_color "bpy.types.Node.use_custom_color")
  * [`Node.color`](bpy.types.Node.html#bpy.types.Node.color "bpy.types.Node.color")
  * [`Node.color_tag`](bpy.types.Node.html#bpy.types.Node.color_tag "bpy.types.Node.color_tag")

| 

  * [`Node.select`](bpy.types.Node.html#bpy.types.Node.select "bpy.types.Node.select")
  * [`Node.show_options`](bpy.types.Node.html#bpy.types.Node.show_options "bpy.types.Node.show_options")
  * [`Node.show_preview`](bpy.types.Node.html#bpy.types.Node.show_preview "bpy.types.Node.show_preview")
  * [`Node.hide`](bpy.types.Node.html#bpy.types.Node.hide "bpy.types.Node.hide")
  * [`Node.mute`](bpy.types.Node.html#bpy.types.Node.mute "bpy.types.Node.mute")
  * [`Node.show_texture`](bpy.types.Node.html#bpy.types.Node.show_texture "bpy.types.Node.show_texture")
  * [`Node.bl_idname`](bpy.types.Node.html#bpy.types.Node.bl_idname "bpy.types.Node.bl_idname")
  * [`Node.bl_label`](bpy.types.Node.html#bpy.types.Node.bl_label "bpy.types.Node.bl_label")
  * [`Node.bl_description`](bpy.types.Node.html#bpy.types.Node.bl_description "bpy.types.Node.bl_description")
  * [`Node.bl_icon`](bpy.types.Node.html#bpy.types.Node.bl_icon "bpy.types.Node.bl_icon")
  * [`Node.bl_static_type`](bpy.types.Node.html#bpy.types.Node.bl_static_type "bpy.types.Node.bl_static_type")
  * [`Node.bl_width_default`](bpy.types.Node.html#bpy.types.Node.bl_width_default "bpy.types.Node.bl_width_default")
  * [`Node.bl_width_min`](bpy.types.Node.html#bpy.types.Node.bl_width_min "bpy.types.Node.bl_width_min")
  * [`Node.bl_width_max`](bpy.types.Node.html#bpy.types.Node.bl_width_max "bpy.types.Node.bl_width_max")
  * [`Node.bl_height_default`](bpy.types.Node.html#bpy.types.Node.bl_height_default "bpy.types.Node.bl_height_default")
  * [`Node.bl_height_min`](bpy.types.Node.html#bpy.types.Node.bl_height_min "bpy.types.Node.bl_height_min")
  * [`Node.bl_height_max`](bpy.types.Node.html#bpy.types.Node.bl_height_max "bpy.types.Node.bl_height_max")

  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`Node.socket_value_update`](bpy.types.Node.html#bpy.types.Node.socket_value_update "bpy.types.Node.socket_value_update")

| 

  * [`Node.is_registered_node_type`](bpy.types.Node.html#bpy.types.Node.is_registered_node_type "bpy.types.Node.is_registered_node_type")
  * [`Node.poll`](bpy.types.Node.html#bpy.types.Node.poll "bpy.types.Node.poll")
  * [`Node.poll_instance`](bpy.types.Node.html#bpy.types.Node.poll_instance "bpy.types.Node.poll_instance")
  * [`Node.update`](bpy.types.Node.html#bpy.types.Node.update "bpy.types.Node.update")
  * [`Node.insert_link`](bpy.types.Node.html#bpy.types.Node.insert_link "bpy.types.Node.insert_link")
  * [`Node.init`](bpy.types.Node.html#bpy.types.Node.init "bpy.types.Node.init")
  * [`Node.copy`](bpy.types.Node.html#bpy.types.Node.copy "bpy.types.Node.copy")
  * [`Node.free`](bpy.types.Node.html#bpy.types.Node.free "bpy.types.Node.free")
  * [`Node.draw_buttons`](bpy.types.Node.html#bpy.types.Node.draw_buttons "bpy.types.Node.draw_buttons")
  * [`Node.draw_buttons_ext`](bpy.types.Node.html#bpy.types.Node.draw_buttons_ext "bpy.types.Node.draw_buttons_ext")
  * [`Node.draw_label`](bpy.types.Node.html#bpy.types.Node.draw_label "bpy.types.Node.draw_label")
  * [`Node.debug_zone_body_lazy_function_graph`](bpy.types.Node.html#bpy.types.Node.debug_zone_body_lazy_function_graph "bpy.types.Node.debug_zone_body_lazy_function_graph")
  * [`Node.debug_zone_lazy_function_graph`](bpy.types.Node.html#bpy.types.Node.debug_zone_lazy_function_graph "bpy.types.Node.debug_zone_lazy_function_graph")
  * [`Node.poll`](bpy.types.Node.html#bpy.types.Node.poll "bpy.types.Node.poll")
  * [`Node.bl_rna_get_subclass`](bpy.types.Node.html#bpy.types.Node.bl_rna_get_subclass "bpy.types.Node.bl_rna_get_subclass")
  * [`Node.bl_rna_get_subclass_py`](bpy.types.Node.html#bpy.types.Node.bl_rna_get_subclass_py "bpy.types.Node.bl_rna_get_subclass_py")
  * [`NodeInternal.poll`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.poll "bpy.types.NodeInternal.poll")
  * [`NodeInternal.poll_instance`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.poll_instance "bpy.types.NodeInternal.poll_instance")
  * [`NodeInternal.update`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.update "bpy.types.NodeInternal.update")
  * [`NodeInternal.draw_buttons`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.draw_buttons "bpy.types.NodeInternal.draw_buttons")
  * [`NodeInternal.draw_buttons_ext`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.draw_buttons_ext "bpy.types.NodeInternal.draw_buttons_ext")
  * [`NodeInternal.bl_rna_get_subclass`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.bl_rna_get_subclass "bpy.types.NodeInternal.bl_rna_get_subclass")
  * [`NodeInternal.bl_rna_get_subclass_py`](bpy.types.NodeInternal.html#bpy.types.NodeInternal.bl_rna_get_subclass_py "bpy.types.NodeInternal.bl_rna_get_subclass_py")

  
---|---
