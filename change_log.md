# Change Log

Changes in Blender’s Python API between releases.

## 4.4 to 4.5

### bpy.types.AnimData

#### Added

  * [`bpy.types.AnimData.action_slot_handle_tweak_storage`](bpy.types.AnimData.md#bpy.types.AnimData.action_slot_handle_tweak_storage "bpy.types.AnimData.action_slot_handle_tweak_storage")


### bpy.types.Bone

#### Added

  * [`bpy.types.Bone.display_type`](bpy.types.Bone.md#bpy.types.Bone.display_type "bpy.types.Bone.display_type")


### bpy.types.Brush

#### Added

  * [`bpy.types.Brush.curve_random_hue`](bpy.types.Brush.md#bpy.types.Brush.curve_random_hue "bpy.types.Brush.curve_random_hue")

  * [`bpy.types.Brush.curve_random_saturation`](bpy.types.Brush.md#bpy.types.Brush.curve_random_saturation "bpy.types.Brush.curve_random_saturation")

  * [`bpy.types.Brush.curve_random_value`](bpy.types.Brush.md#bpy.types.Brush.curve_random_value "bpy.types.Brush.curve_random_value")

  * [`bpy.types.Brush.hue_jitter`](bpy.types.Brush.md#bpy.types.Brush.hue_jitter "bpy.types.Brush.hue_jitter")

  * [`bpy.types.Brush.saturation_jitter`](bpy.types.Brush.md#bpy.types.Brush.saturation_jitter "bpy.types.Brush.saturation_jitter")

  * [`bpy.types.Brush.use_color_jitter`](bpy.types.Brush.md#bpy.types.Brush.use_color_jitter "bpy.types.Brush.use_color_jitter")

  * [`bpy.types.Brush.use_random_press_hue`](bpy.types.Brush.md#bpy.types.Brush.use_random_press_hue "bpy.types.Brush.use_random_press_hue")

  * [`bpy.types.Brush.use_random_press_sat`](bpy.types.Brush.md#bpy.types.Brush.use_random_press_sat "bpy.types.Brush.use_random_press_sat")

  * [`bpy.types.Brush.use_random_press_val`](bpy.types.Brush.md#bpy.types.Brush.use_random_press_val "bpy.types.Brush.use_random_press_val")

  * [`bpy.types.Brush.use_stroke_random_hue`](bpy.types.Brush.md#bpy.types.Brush.use_stroke_random_hue "bpy.types.Brush.use_stroke_random_hue")

  * [`bpy.types.Brush.use_stroke_random_sat`](bpy.types.Brush.md#bpy.types.Brush.use_stroke_random_sat "bpy.types.Brush.use_stroke_random_sat")

  * [`bpy.types.Brush.use_stroke_random_val`](bpy.types.Brush.md#bpy.types.Brush.use_stroke_random_val "bpy.types.Brush.use_stroke_random_val")

  * [`bpy.types.Brush.value_jitter`](bpy.types.Brush.md#bpy.types.Brush.value_jitter "bpy.types.Brush.value_jitter")


### bpy.types.BrushCapabilitiesSculpt

#### Added

  * [`bpy.types.BrushCapabilitiesSculpt.has_dyntopo`](bpy.types.BrushCapabilitiesSculpt.md#bpy.types.BrushCapabilitiesSculpt.has_dyntopo "bpy.types.BrushCapabilitiesSculpt.has_dyntopo")


### bpy.types.BrushGpencilSettings

#### Added

  * [`bpy.types.BrushGpencilSettings.use_auto_remove_fill_guides`](bpy.types.BrushGpencilSettings.md#bpy.types.BrushGpencilSettings.use_auto_remove_fill_guides "bpy.types.BrushGpencilSettings.use_auto_remove_fill_guides")


### bpy.types.CYCLES

#### Added

  * `bpy.types.CYCLES.update_custom_camera`


### bpy.types.Camera

#### Added

  * [`bpy.types.Camera.custom_bytecode`](bpy.types.Camera.md#bpy.types.Camera.custom_bytecode "bpy.types.Camera.custom_bytecode")

  * [`bpy.types.Camera.custom_bytecode_hash`](bpy.types.Camera.md#bpy.types.Camera.custom_bytecode_hash "bpy.types.Camera.custom_bytecode_hash")

  * [`bpy.types.Camera.custom_filepath`](bpy.types.Camera.md#bpy.types.Camera.custom_filepath "bpy.types.Camera.custom_filepath")

  * [`bpy.types.Camera.custom_mode`](bpy.types.Camera.md#bpy.types.Camera.custom_mode "bpy.types.Camera.custom_mode")

  * [`bpy.types.Camera.custom_shader`](bpy.types.Camera.md#bpy.types.Camera.custom_shader "bpy.types.Camera.custom_shader")

  * [`bpy.types.Camera.cycles_custom`](bpy.types.Camera.md#bpy.types.Camera.cycles_custom "bpy.types.Camera.cycles_custom")


### bpy.types.CollectionExport

#### Added

  * [`bpy.types.CollectionExport.filepath`](bpy.types.CollectionExport.md#bpy.types.CollectionExport.filepath "bpy.types.CollectionExport.filepath")


### bpy.types.CompositorNodeCornerPin

#### Added

  * [`bpy.types.CompositorNodeCornerPin.interpolation`](bpy.types.CompositorNodeCornerPin.md#bpy.types.CompositorNodeCornerPin.interpolation "bpy.types.CompositorNodeCornerPin.interpolation")


### bpy.types.CompositorNodeLensdist

#### Added

  * [`bpy.types.CompositorNodeLensdist.distortion_type`](bpy.types.CompositorNodeLensdist.md#bpy.types.CompositorNodeLensdist.distortion_type "bpy.types.CompositorNodeLensdist.distortion_type")


### bpy.types.CompositorNodeScale

#### Added

  * [`bpy.types.CompositorNodeScale.interpolation`](bpy.types.CompositorNodeScale.md#bpy.types.CompositorNodeScale.interpolation "bpy.types.CompositorNodeScale.interpolation")


### bpy.types.CyclesPreferences

#### Function Arguments

  * `bpy.types.CyclesPreferences.get_devices_for_type` (self, compute_device_type, device_list), _was (self, compute_device_type)_


### bpy.types.DopeSheet

#### Added

  * [`bpy.types.DopeSheet.show_lightprobes`](bpy.types.DopeSheet.md#bpy.types.DopeSheet.show_lightprobes "bpy.types.DopeSheet.show_lightprobes")


### bpy.types.EditBone

#### Added

  * [`bpy.types.EditBone.display_type`](bpy.types.EditBone.md#bpy.types.EditBone.display_type "bpy.types.EditBone.display_type")


### bpy.types.Event

#### Added

  * [`bpy.types.Event.hyper`](bpy.types.Event.md#bpy.types.Event.hyper "bpy.types.Event.hyper")

  * [`bpy.types.Event.ndof_motion`](bpy.types.Event.md#bpy.types.Event.ndof_motion "bpy.types.Event.ndof_motion")


### bpy.types.FFmpegSettings

#### Added

  * [`bpy.types.FFmpegSettings.ffmpeg_prores_profile`](bpy.types.FFmpegSettings.md#bpy.types.FFmpegSettings.ffmpeg_prores_profile "bpy.types.FFmpegSettings.ffmpeg_prores_profile")


### bpy.types.FileAssetSelectParams

#### Added

  * [`bpy.types.FileAssetSelectParams.instance_collections_on_append`](bpy.types.FileAssetSelectParams.md#bpy.types.FileAssetSelectParams.instance_collections_on_append "bpy.types.FileAssetSelectParams.instance_collections_on_append")

  * [`bpy.types.FileAssetSelectParams.instance_collections_on_link`](bpy.types.FileAssetSelectParams.md#bpy.types.FileAssetSelectParams.instance_collections_on_link "bpy.types.FileAssetSelectParams.instance_collections_on_link")


### bpy.types.FileSelectParams

#### Added

  * [`bpy.types.FileSelectParams.list_column_size`](bpy.types.FileSelectParams.md#bpy.types.FileSelectParams.list_column_size "bpy.types.FileSelectParams.list_column_size")

  * [`bpy.types.FileSelectParams.list_display_size`](bpy.types.FileSelectParams.md#bpy.types.FileSelectParams.list_display_size "bpy.types.FileSelectParams.list_display_size")


### bpy.types.GeometryNodeMeshToCurve

#### Added

  * [`bpy.types.GeometryNodeMeshToCurve.mode`](bpy.types.GeometryNodeMeshToCurve.md#bpy.types.GeometryNodeMeshToCurve.mode "bpy.types.GeometryNodeMeshToCurve.mode")


### bpy.types.GeometryNodeTree

#### Renamed

  * **is_type_point_cloud** -> [`bpy.types.GeometryNodeTree.is_mode_paint`](bpy.types.GeometryNodeTree.md#bpy.types.GeometryNodeTree.is_mode_paint "bpy.types.GeometryNodeTree.is_mode_paint")

  * **is_type_point_cloud** -> [`bpy.types.GeometryNodeTree.is_type_grease_pencil`](bpy.types.GeometryNodeTree.md#bpy.types.GeometryNodeTree.is_type_grease_pencil "bpy.types.GeometryNodeTree.is_type_grease_pencil")

  * **is_type_point_cloud** -> [`bpy.types.GeometryNodeTree.is_type_pointcloud`](bpy.types.GeometryNodeTree.md#bpy.types.GeometryNodeTree.is_type_pointcloud "bpy.types.GeometryNodeTree.is_type_pointcloud")


### bpy.types.GeometryNodeViewer

#### Added

  * [`bpy.types.GeometryNodeViewer.ui_shortcut`](bpy.types.GeometryNodeViewer.md#bpy.types.GeometryNodeViewer.ui_shortcut "bpy.types.GeometryNodeViewer.ui_shortcut")


### bpy.types.GreasePencilArrayModifier

#### Added

  * [`bpy.types.GreasePencilArrayModifier.use_layer_group_filter`](bpy.types.GreasePencilArrayModifier.md#bpy.types.GreasePencilArrayModifier.use_layer_group_filter "bpy.types.GreasePencilArrayModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilArrayModifier.tree_node_filter`](bpy.types.GreasePencilArrayModifier.md#bpy.types.GreasePencilArrayModifier.tree_node_filter "bpy.types.GreasePencilArrayModifier.tree_node_filter")


### bpy.types.GreasePencilBuildModifier

#### Added

  * [`bpy.types.GreasePencilBuildModifier.use_layer_group_filter`](bpy.types.GreasePencilBuildModifier.md#bpy.types.GreasePencilBuildModifier.use_layer_group_filter "bpy.types.GreasePencilBuildModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilBuildModifier.tree_node_filter`](bpy.types.GreasePencilBuildModifier.md#bpy.types.GreasePencilBuildModifier.tree_node_filter "bpy.types.GreasePencilBuildModifier.tree_node_filter")


### bpy.types.GreasePencilColorModifier

#### Added

  * [`bpy.types.GreasePencilColorModifier.use_layer_group_filter`](bpy.types.GreasePencilColorModifier.md#bpy.types.GreasePencilColorModifier.use_layer_group_filter "bpy.types.GreasePencilColorModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilColorModifier.tree_node_filter`](bpy.types.GreasePencilColorModifier.md#bpy.types.GreasePencilColorModifier.tree_node_filter "bpy.types.GreasePencilColorModifier.tree_node_filter")


### bpy.types.GreasePencilDashModifierData

#### Added

  * [`bpy.types.GreasePencilDashModifierData.use_layer_group_filter`](bpy.types.GreasePencilDashModifierData.md#bpy.types.GreasePencilDashModifierData.use_layer_group_filter "bpy.types.GreasePencilDashModifierData.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilDashModifierData.tree_node_filter`](bpy.types.GreasePencilDashModifierData.md#bpy.types.GreasePencilDashModifierData.tree_node_filter "bpy.types.GreasePencilDashModifierData.tree_node_filter")


### bpy.types.GreasePencilDrawing

#### Added

  * [`bpy.types.GreasePencilDrawing.set_vertex_weights`](bpy.types.GreasePencilDrawing.md#bpy.types.GreasePencilDrawing.set_vertex_weights "bpy.types.GreasePencilDrawing.set_vertex_weights")

  * [`bpy.types.GreasePencilDrawing.vertex_group_assign`](bpy.types.GreasePencilDrawing.md#bpy.types.GreasePencilDrawing.vertex_group_assign "bpy.types.GreasePencilDrawing.vertex_group_assign")

  * [`bpy.types.GreasePencilDrawing.vertex_group_remove`](bpy.types.GreasePencilDrawing.md#bpy.types.GreasePencilDrawing.vertex_group_remove "bpy.types.GreasePencilDrawing.vertex_group_remove")


### bpy.types.GreasePencilEnvelopeModifier

#### Added

  * [`bpy.types.GreasePencilEnvelopeModifier.use_layer_group_filter`](bpy.types.GreasePencilEnvelopeModifier.md#bpy.types.GreasePencilEnvelopeModifier.use_layer_group_filter "bpy.types.GreasePencilEnvelopeModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilEnvelopeModifier.tree_node_filter`](bpy.types.GreasePencilEnvelopeModifier.md#bpy.types.GreasePencilEnvelopeModifier.tree_node_filter "bpy.types.GreasePencilEnvelopeModifier.tree_node_filter")


### bpy.types.GreasePencilHookModifier

#### Added

  * [`bpy.types.GreasePencilHookModifier.use_layer_group_filter`](bpy.types.GreasePencilHookModifier.md#bpy.types.GreasePencilHookModifier.use_layer_group_filter "bpy.types.GreasePencilHookModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilHookModifier.tree_node_filter`](bpy.types.GreasePencilHookModifier.md#bpy.types.GreasePencilHookModifier.tree_node_filter "bpy.types.GreasePencilHookModifier.tree_node_filter")


### bpy.types.GreasePencilLatticeModifier

#### Added

  * [`bpy.types.GreasePencilLatticeModifier.use_layer_group_filter`](bpy.types.GreasePencilLatticeModifier.md#bpy.types.GreasePencilLatticeModifier.use_layer_group_filter "bpy.types.GreasePencilLatticeModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilLatticeModifier.tree_node_filter`](bpy.types.GreasePencilLatticeModifier.md#bpy.types.GreasePencilLatticeModifier.tree_node_filter "bpy.types.GreasePencilLatticeModifier.tree_node_filter")


### bpy.types.GreasePencilLengthModifier

#### Added

  * [`bpy.types.GreasePencilLengthModifier.use_layer_group_filter`](bpy.types.GreasePencilLengthModifier.md#bpy.types.GreasePencilLengthModifier.use_layer_group_filter "bpy.types.GreasePencilLengthModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilLengthModifier.tree_node_filter`](bpy.types.GreasePencilLengthModifier.md#bpy.types.GreasePencilLengthModifier.tree_node_filter "bpy.types.GreasePencilLengthModifier.tree_node_filter")


### bpy.types.GreasePencilLineartModifier

#### Added

  * [`bpy.types.GreasePencilLineartModifier.radius`](bpy.types.GreasePencilLineartModifier.md#bpy.types.GreasePencilLineartModifier.radius "bpy.types.GreasePencilLineartModifier.radius")


### bpy.types.GreasePencilMirrorModifier

#### Added

  * [`bpy.types.GreasePencilMirrorModifier.use_layer_group_filter`](bpy.types.GreasePencilMirrorModifier.md#bpy.types.GreasePencilMirrorModifier.use_layer_group_filter "bpy.types.GreasePencilMirrorModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilMirrorModifier.tree_node_filter`](bpy.types.GreasePencilMirrorModifier.md#bpy.types.GreasePencilMirrorModifier.tree_node_filter "bpy.types.GreasePencilMirrorModifier.tree_node_filter")


### bpy.types.GreasePencilMultiplyModifier

#### Added

  * [`bpy.types.GreasePencilMultiplyModifier.use_layer_group_filter`](bpy.types.GreasePencilMultiplyModifier.md#bpy.types.GreasePencilMultiplyModifier.use_layer_group_filter "bpy.types.GreasePencilMultiplyModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilMultiplyModifier.tree_node_filter`](bpy.types.GreasePencilMultiplyModifier.md#bpy.types.GreasePencilMultiplyModifier.tree_node_filter "bpy.types.GreasePencilMultiplyModifier.tree_node_filter")


### bpy.types.GreasePencilNoiseModifier

#### Added

  * [`bpy.types.GreasePencilNoiseModifier.use_layer_group_filter`](bpy.types.GreasePencilNoiseModifier.md#bpy.types.GreasePencilNoiseModifier.use_layer_group_filter "bpy.types.GreasePencilNoiseModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilNoiseModifier.tree_node_filter`](bpy.types.GreasePencilNoiseModifier.md#bpy.types.GreasePencilNoiseModifier.tree_node_filter "bpy.types.GreasePencilNoiseModifier.tree_node_filter")


### bpy.types.GreasePencilOffsetModifier

#### Added

  * [`bpy.types.GreasePencilOffsetModifier.use_layer_group_filter`](bpy.types.GreasePencilOffsetModifier.md#bpy.types.GreasePencilOffsetModifier.use_layer_group_filter "bpy.types.GreasePencilOffsetModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilOffsetModifier.tree_node_filter`](bpy.types.GreasePencilOffsetModifier.md#bpy.types.GreasePencilOffsetModifier.tree_node_filter "bpy.types.GreasePencilOffsetModifier.tree_node_filter")


### bpy.types.GreasePencilOpacityModifier

#### Added

  * [`bpy.types.GreasePencilOpacityModifier.use_layer_group_filter`](bpy.types.GreasePencilOpacityModifier.md#bpy.types.GreasePencilOpacityModifier.use_layer_group_filter "bpy.types.GreasePencilOpacityModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilOpacityModifier.tree_node_filter`](bpy.types.GreasePencilOpacityModifier.md#bpy.types.GreasePencilOpacityModifier.tree_node_filter "bpy.types.GreasePencilOpacityModifier.tree_node_filter")


### bpy.types.GreasePencilOutlineModifier

#### Added

  * [`bpy.types.GreasePencilOutlineModifier.use_layer_group_filter`](bpy.types.GreasePencilOutlineModifier.md#bpy.types.GreasePencilOutlineModifier.use_layer_group_filter "bpy.types.GreasePencilOutlineModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilOutlineModifier.tree_node_filter`](bpy.types.GreasePencilOutlineModifier.md#bpy.types.GreasePencilOutlineModifier.tree_node_filter "bpy.types.GreasePencilOutlineModifier.tree_node_filter")


### bpy.types.GreasePencilShrinkwrapModifier

#### Added

  * [`bpy.types.GreasePencilShrinkwrapModifier.use_layer_group_filter`](bpy.types.GreasePencilShrinkwrapModifier.md#bpy.types.GreasePencilShrinkwrapModifier.use_layer_group_filter "bpy.types.GreasePencilShrinkwrapModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilShrinkwrapModifier.tree_node_filter`](bpy.types.GreasePencilShrinkwrapModifier.md#bpy.types.GreasePencilShrinkwrapModifier.tree_node_filter "bpy.types.GreasePencilShrinkwrapModifier.tree_node_filter")


### bpy.types.GreasePencilSimplifyModifier

#### Added

  * [`bpy.types.GreasePencilSimplifyModifier.use_layer_group_filter`](bpy.types.GreasePencilSimplifyModifier.md#bpy.types.GreasePencilSimplifyModifier.use_layer_group_filter "bpy.types.GreasePencilSimplifyModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilSimplifyModifier.tree_node_filter`](bpy.types.GreasePencilSimplifyModifier.md#bpy.types.GreasePencilSimplifyModifier.tree_node_filter "bpy.types.GreasePencilSimplifyModifier.tree_node_filter")


### bpy.types.GreasePencilSmoothModifier

#### Added

  * [`bpy.types.GreasePencilSmoothModifier.use_layer_group_filter`](bpy.types.GreasePencilSmoothModifier.md#bpy.types.GreasePencilSmoothModifier.use_layer_group_filter "bpy.types.GreasePencilSmoothModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilSmoothModifier.tree_node_filter`](bpy.types.GreasePencilSmoothModifier.md#bpy.types.GreasePencilSmoothModifier.tree_node_filter "bpy.types.GreasePencilSmoothModifier.tree_node_filter")


### bpy.types.GreasePencilSubdivModifier

#### Added

  * [`bpy.types.GreasePencilSubdivModifier.use_layer_group_filter`](bpy.types.GreasePencilSubdivModifier.md#bpy.types.GreasePencilSubdivModifier.use_layer_group_filter "bpy.types.GreasePencilSubdivModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilSubdivModifier.tree_node_filter`](bpy.types.GreasePencilSubdivModifier.md#bpy.types.GreasePencilSubdivModifier.tree_node_filter "bpy.types.GreasePencilSubdivModifier.tree_node_filter")


### bpy.types.GreasePencilTextureModifier

#### Added

  * [`bpy.types.GreasePencilTextureModifier.use_layer_group_filter`](bpy.types.GreasePencilTextureModifier.md#bpy.types.GreasePencilTextureModifier.use_layer_group_filter "bpy.types.GreasePencilTextureModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilTextureModifier.tree_node_filter`](bpy.types.GreasePencilTextureModifier.md#bpy.types.GreasePencilTextureModifier.tree_node_filter "bpy.types.GreasePencilTextureModifier.tree_node_filter")


### bpy.types.GreasePencilThickModifierData

#### Added

  * [`bpy.types.GreasePencilThickModifierData.use_layer_group_filter`](bpy.types.GreasePencilThickModifierData.md#bpy.types.GreasePencilThickModifierData.use_layer_group_filter "bpy.types.GreasePencilThickModifierData.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilThickModifierData.tree_node_filter`](bpy.types.GreasePencilThickModifierData.md#bpy.types.GreasePencilThickModifierData.tree_node_filter "bpy.types.GreasePencilThickModifierData.tree_node_filter")


### bpy.types.GreasePencilTimeModifier

#### Added

  * [`bpy.types.GreasePencilTimeModifier.use_layer_group_filter`](bpy.types.GreasePencilTimeModifier.md#bpy.types.GreasePencilTimeModifier.use_layer_group_filter "bpy.types.GreasePencilTimeModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilTimeModifier.tree_node_filter`](bpy.types.GreasePencilTimeModifier.md#bpy.types.GreasePencilTimeModifier.tree_node_filter "bpy.types.GreasePencilTimeModifier.tree_node_filter")


### bpy.types.GreasePencilTintModifier

#### Added

  * [`bpy.types.GreasePencilTintModifier.use_layer_group_filter`](bpy.types.GreasePencilTintModifier.md#bpy.types.GreasePencilTintModifier.use_layer_group_filter "bpy.types.GreasePencilTintModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilTintModifier.tree_node_filter`](bpy.types.GreasePencilTintModifier.md#bpy.types.GreasePencilTintModifier.tree_node_filter "bpy.types.GreasePencilTintModifier.tree_node_filter")


### bpy.types.GreasePencilWeightAngleModifier

#### Added

  * [`bpy.types.GreasePencilWeightAngleModifier.use_layer_group_filter`](bpy.types.GreasePencilWeightAngleModifier.md#bpy.types.GreasePencilWeightAngleModifier.use_layer_group_filter "bpy.types.GreasePencilWeightAngleModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilWeightAngleModifier.tree_node_filter`](bpy.types.GreasePencilWeightAngleModifier.md#bpy.types.GreasePencilWeightAngleModifier.tree_node_filter "bpy.types.GreasePencilWeightAngleModifier.tree_node_filter")


### bpy.types.GreasePencilWeightProximityModifier

#### Added

  * [`bpy.types.GreasePencilWeightProximityModifier.use_layer_group_filter`](bpy.types.GreasePencilWeightProximityModifier.md#bpy.types.GreasePencilWeightProximityModifier.use_layer_group_filter "bpy.types.GreasePencilWeightProximityModifier.use_layer_group_filter")


#### Renamed

  * **layer_filter** -> [`bpy.types.GreasePencilWeightProximityModifier.tree_node_filter`](bpy.types.GreasePencilWeightProximityModifier.md#bpy.types.GreasePencilWeightProximityModifier.tree_node_filter "bpy.types.GreasePencilWeightProximityModifier.tree_node_filter")


### bpy.types.KeyMapItem

#### Added

  * [`bpy.types.KeyMapItem.hyper`](bpy.types.KeyMapItem.md#bpy.types.KeyMapItem.hyper "bpy.types.KeyMapItem.hyper")

  * [`bpy.types.KeyMapItem.hyper_ui`](bpy.types.KeyMapItem.md#bpy.types.KeyMapItem.hyper_ui "bpy.types.KeyMapItem.hyper_ui")


### bpy.types.KeyMapItems

#### Added

  * [`bpy.types.KeyMapItems.find_match`](bpy.types.KeyMapItems.md#bpy.types.KeyMapItems.find_match "bpy.types.KeyMapItems.find_match")


#### Function Arguments

  * [`bpy.types.KeyMapItems.new`](bpy.types.KeyMapItems.md#bpy.types.KeyMapItems.new "bpy.types.KeyMapItems.new") (idname, type, value, any, shift, ctrl, alt, oskey, hyper, key_modifier, direction, repeat, head), _was (idname, type, value, any, shift, ctrl, alt, oskey, key_modifier, direction, repeat, head)_

  * [`bpy.types.KeyMapItems.new_modal`](bpy.types.KeyMapItems.md#bpy.types.KeyMapItems.new_modal "bpy.types.KeyMapItems.new_modal") (propvalue, type, value, any, shift, ctrl, alt, oskey, hyper, key_modifier, direction, repeat), _was (propvalue, type, value, any, shift, ctrl, alt, oskey, key_modifier, direction, repeat)_


### bpy.types.KeyMaps

#### Added

  * [`bpy.types.KeyMaps.find_match`](bpy.types.KeyMaps.md#bpy.types.KeyMaps.find_match "bpy.types.KeyMaps.find_match")


### bpy.types.Light

#### Added

  * [`bpy.types.Light.area`](bpy.types.Light.md#bpy.types.Light.area "bpy.types.Light.area")

  * [`bpy.types.Light.exposure`](bpy.types.Light.md#bpy.types.Light.exposure "bpy.types.Light.exposure")

  * [`bpy.types.Light.normalize`](bpy.types.Light.md#bpy.types.Light.normalize "bpy.types.Light.normalize")

  * [`bpy.types.Light.temperature`](bpy.types.Light.md#bpy.types.Light.temperature "bpy.types.Light.temperature")

  * [`bpy.types.Light.temperature_color`](bpy.types.Light.md#bpy.types.Light.temperature_color "bpy.types.Light.temperature_color")

  * [`bpy.types.Light.use_temperature`](bpy.types.Light.md#bpy.types.Light.use_temperature "bpy.types.Light.use_temperature")


### bpy.types.Mesh

#### Function Arguments

  * [`bpy.types.Mesh.calc_smooth_groups`](bpy.types.Mesh.md#bpy.types.Mesh.calc_smooth_groups "bpy.types.Mesh.calc_smooth_groups") (use_bitflags, use_boundary_vertices_for_bitflags), _was (use_bitflags)_


### bpy.types.ModifierViewerPathElem

#### Added

  * [`bpy.types.ModifierViewerPathElem.modifier_uid`](bpy.types.ModifierViewerPathElem.md#bpy.types.ModifierViewerPathElem.modifier_uid "bpy.types.ModifierViewerPathElem.modifier_uid")


#### Removed

  * **modifier_name**


### bpy.types.NodeSocket

#### Added

  * [`bpy.types.NodeSocket.is_icon_visible`](bpy.types.NodeSocket.md#bpy.types.NodeSocket.is_icon_visible "bpy.types.NodeSocket.is_icon_visible")

  * [`bpy.types.NodeSocket.is_inactive`](bpy.types.NodeSocket.md#bpy.types.NodeSocket.is_inactive "bpy.types.NodeSocket.is_inactive")

  * [`bpy.types.NodeSocket.select`](bpy.types.NodeSocket.md#bpy.types.NodeSocket.select "bpy.types.NodeSocket.select")


### bpy.types.NodeTreeInterfaceSocket

#### Added

  * [`bpy.types.NodeTreeInterfaceSocket.is_panel_toggle`](bpy.types.NodeTreeInterfaceSocket.md#bpy.types.NodeTreeInterfaceSocket.is_panel_toggle "bpy.types.NodeTreeInterfaceSocket.is_panel_toggle")

  * [`bpy.types.NodeTreeInterfaceSocket.menu_expanded`](bpy.types.NodeTreeInterfaceSocket.md#bpy.types.NodeTreeInterfaceSocket.menu_expanded "bpy.types.NodeTreeInterfaceSocket.menu_expanded")

  * [`bpy.types.NodeTreeInterfaceSocket.structure_type`](bpy.types.NodeTreeInterfaceSocket.md#bpy.types.NodeTreeInterfaceSocket.structure_type "bpy.types.NodeTreeInterfaceSocket.structure_type")


### bpy.types.NodeTreeInterfaceSocketVector

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVector.dimensions`](bpy.types.NodeTreeInterfaceSocketVector.md#bpy.types.NodeTreeInterfaceSocketVector.dimensions "bpy.types.NodeTreeInterfaceSocketVector.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorAcceleration

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorAcceleration.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorAcceleration.md#bpy.types.NodeTreeInterfaceSocketVectorAcceleration.dimensions "bpy.types.NodeTreeInterfaceSocketVectorAcceleration.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorDirection

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorDirection.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorDirection.md#bpy.types.NodeTreeInterfaceSocketVectorDirection.dimensions "bpy.types.NodeTreeInterfaceSocketVectorDirection.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorEuler

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorEuler.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorEuler.md#bpy.types.NodeTreeInterfaceSocketVectorEuler.dimensions "bpy.types.NodeTreeInterfaceSocketVectorEuler.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorTranslation

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorTranslation.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorTranslation.md#bpy.types.NodeTreeInterfaceSocketVectorTranslation.dimensions "bpy.types.NodeTreeInterfaceSocketVectorTranslation.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorVelocity

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorVelocity.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorVelocity.md#bpy.types.NodeTreeInterfaceSocketVectorVelocity.dimensions "bpy.types.NodeTreeInterfaceSocketVectorVelocity.dimensions")


### bpy.types.NodeTreeInterfaceSocketVectorXYZ

#### Added

  * [`bpy.types.NodeTreeInterfaceSocketVectorXYZ.dimensions`](bpy.types.NodeTreeInterfaceSocketVectorXYZ.md#bpy.types.NodeTreeInterfaceSocketVectorXYZ.dimensions "bpy.types.NodeTreeInterfaceSocketVectorXYZ.dimensions")


### bpy.types.Object

#### Added

  * [`bpy.types.Object.evaluated_geometry`](bpy.types.Object.md#bpy.types.Object.evaluated_geometry "bpy.types.Object.evaluated_geometry")

  * [`bpy.types.Object.shadow_terminator_geometry_offset`](bpy.types.Object.md#bpy.types.Object.shadow_terminator_geometry_offset "bpy.types.Object.shadow_terminator_geometry_offset")

  * [`bpy.types.Object.shadow_terminator_normal_offset`](bpy.types.Object.md#bpy.types.Object.shadow_terminator_normal_offset "bpy.types.Object.shadow_terminator_normal_offset")

  * [`bpy.types.Object.shadow_terminator_shading_offset`](bpy.types.Object.md#bpy.types.Object.shadow_terminator_shading_offset "bpy.types.Object.shadow_terminator_shading_offset")

  * [`bpy.types.Object.use_parent_final_indices`](bpy.types.Object.md#bpy.types.Object.use_parent_final_indices "bpy.types.Object.use_parent_final_indices")


### bpy.types.PreferencesExperimental

#### Removed

  * **use_new_file_import_nodes**

  * **use_new_point_cloud_type**


#### Renamed

  * **use_sculpt_tools_tilt** -> [`bpy.types.PreferencesExperimental.use_attribute_storage_write`](bpy.types.PreferencesExperimental.md#bpy.types.PreferencesExperimental.use_attribute_storage_write "bpy.types.PreferencesExperimental.use_attribute_storage_write")

  * **use_sculpt_tools_tilt** -> [`bpy.types.PreferencesExperimental.use_bundle_and_closure_nodes`](bpy.types.PreferencesExperimental.md#bpy.types.PreferencesExperimental.use_bundle_and_closure_nodes "bpy.types.PreferencesExperimental.use_bundle_and_closure_nodes")

  * **use_sculpt_tools_tilt** -> [`bpy.types.PreferencesExperimental.use_socket_structure_type`](bpy.types.PreferencesExperimental.md#bpy.types.PreferencesExperimental.use_socket_structure_type "bpy.types.PreferencesExperimental.use_socket_structure_type")

  * **use_sculpt_tools_tilt** -> [`bpy.types.PreferencesExperimental.write_large_blend_file_blocks`](bpy.types.PreferencesExperimental.md#bpy.types.PreferencesExperimental.write_large_blend_file_blocks "bpy.types.PreferencesExperimental.write_large_blend_file_blocks")


### bpy.types.PreferencesInput

#### Added

  * [`bpy.types.PreferencesInput.ndof_zoom_direction`](bpy.types.PreferencesInput.md#bpy.types.PreferencesInput.ndof_zoom_direction "bpy.types.PreferencesInput.ndof_zoom_direction")


#### Removed

  * **ndof_pan_yz_swap_axis**

  * **ndof_view_rotate_method**

  * **ndof_zoom_invert**


#### Renamed

  * **ndof_view_navigate_method** -> [`bpy.types.PreferencesInput.ndof_navigation_mode`](bpy.types.PreferencesInput.md#bpy.types.PreferencesInput.ndof_navigation_mode "bpy.types.PreferencesInput.ndof_navigation_mode")


### bpy.types.PreferencesSystem

#### Added

  * [`bpy.types.PreferencesSystem.gpu_shader_workers`](bpy.types.PreferencesSystem.md#bpy.types.PreferencesSystem.gpu_shader_workers "bpy.types.PreferencesSystem.gpu_shader_workers")

  * [`bpy.types.PreferencesSystem.shader_compilation_method`](bpy.types.PreferencesSystem.md#bpy.types.PreferencesSystem.shader_compilation_method "bpy.types.PreferencesSystem.shader_compilation_method")


#### Removed

  * **max_shader_compilation_subprocesses**

  * **sequencer_disk_cache_compression**

  * **sequencer_disk_cache_dir**

  * **sequencer_disk_cache_size_limit**

  * **use_sequencer_disk_cache**


### bpy.types.PreferencesView

#### Added

  * [`bpy.types.PreferencesView.border_width`](bpy.types.PreferencesView.md#bpy.types.PreferencesView.border_width "bpy.types.PreferencesView.border_width")


### bpy.types.Property

#### Added

  * [`bpy.types.Property.is_path_supports_blend_relative`](bpy.types.Property.md#bpy.types.Property.is_path_supports_blend_relative "bpy.types.Property.is_path_supports_blend_relative")

  * [`bpy.types.Property.is_path_supports_templates`](bpy.types.Property.md#bpy.types.Property.is_path_supports_templates "bpy.types.Property.is_path_supports_templates")


### bpy.types.RenderEngine

#### Added

  * [`bpy.types.RenderEngine.update_custom_camera`](bpy.types.RenderEngine.md#bpy.types.RenderEngine.update_custom_camera "bpy.types.RenderEngine.update_custom_camera")


### bpy.types.RenderLayer

#### Added

  * [`bpy.types.RenderLayer.use_grease_pencil`](bpy.types.RenderLayer.md#bpy.types.RenderLayer.use_grease_pencil "bpy.types.RenderLayer.use_grease_pencil")


### bpy.types.RenderSettings

#### Added

  * [`bpy.types.RenderSettings.compositor_denoise_device`](bpy.types.RenderSettings.md#bpy.types.RenderSettings.compositor_denoise_device "bpy.types.RenderSettings.compositor_denoise_device")

  * [`bpy.types.RenderSettings.ppm_base`](bpy.types.RenderSettings.md#bpy.types.RenderSettings.ppm_base "bpy.types.RenderSettings.ppm_base")

  * [`bpy.types.RenderSettings.ppm_factor`](bpy.types.RenderSettings.md#bpy.types.RenderSettings.ppm_factor "bpy.types.RenderSettings.ppm_factor")


### bpy.types.SceneGpencil

#### Added

  * [`bpy.types.SceneGpencil.aa_samples`](bpy.types.SceneGpencil.md#bpy.types.SceneGpencil.aa_samples "bpy.types.SceneGpencil.aa_samples")

  * [`bpy.types.SceneGpencil.antialias_threshold_render`](bpy.types.SceneGpencil.md#bpy.types.SceneGpencil.antialias_threshold_render "bpy.types.SceneGpencil.antialias_threshold_render")


### bpy.types.SequenceEditor

#### Added

  * [`bpy.types.SequenceEditor.cache_final_size`](bpy.types.SequenceEditor.md#bpy.types.SequenceEditor.cache_final_size "bpy.types.SequenceEditor.cache_final_size")

  * [`bpy.types.SequenceEditor.cache_raw_size`](bpy.types.SequenceEditor.md#bpy.types.SequenceEditor.cache_raw_size "bpy.types.SequenceEditor.cache_raw_size")


#### Removed

  * **use_cache_composite**

  * **use_cache_preprocessed**


### bpy.types.SequencerCacheOverlay

#### Removed

  * **show_cache_composite**

  * **show_cache_preprocessed**


### bpy.types.SequencerToolSettings

#### Added

  * [`bpy.types.SequencerToolSettings.snap_to_frame_range`](bpy.types.SequencerToolSettings.md#bpy.types.SequencerToolSettings.snap_to_frame_range "bpy.types.SequencerToolSettings.snap_to_frame_range")


### bpy.types.SpaceClipEditor

#### Added

  * [`bpy.types.SpaceClipEditor.show_region_channels`](bpy.types.SpaceClipEditor.md#bpy.types.SpaceClipEditor.show_region_channels "bpy.types.SpaceClipEditor.show_region_channels")


### bpy.types.SpaceImageOverlay

#### Added

  * [`bpy.types.SpaceImageOverlay.passepartout_alpha`](bpy.types.SpaceImageOverlay.md#bpy.types.SpaceImageOverlay.passepartout_alpha "bpy.types.SpaceImageOverlay.passepartout_alpha")

  * [`bpy.types.SpaceImageOverlay.show_render_size`](bpy.types.SpaceImageOverlay.md#bpy.types.SpaceImageOverlay.show_render_size "bpy.types.SpaceImageOverlay.show_render_size")

  * [`bpy.types.SpaceImageOverlay.show_text_info`](bpy.types.SpaceImageOverlay.md#bpy.types.SpaceImageOverlay.show_text_info "bpy.types.SpaceImageOverlay.show_text_info")


### bpy.types.SpaceNodeEditor

#### Added

  * [`bpy.types.SpaceNodeEditor.show_gizmo`](bpy.types.SpaceNodeEditor.md#bpy.types.SpaceNodeEditor.show_gizmo "bpy.types.SpaceNodeEditor.show_gizmo")

  * [`bpy.types.SpaceNodeEditor.show_gizmo_active_node`](bpy.types.SpaceNodeEditor.md#bpy.types.SpaceNodeEditor.show_gizmo_active_node "bpy.types.SpaceNodeEditor.show_gizmo_active_node")


### bpy.types.SpaceProperties

#### Added

  * [`bpy.types.SpaceProperties.show_properties_bone`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_bone "bpy.types.SpaceProperties.show_properties_bone")

  * [`bpy.types.SpaceProperties.show_properties_bone_constraints`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_bone_constraints "bpy.types.SpaceProperties.show_properties_bone_constraints")

  * [`bpy.types.SpaceProperties.show_properties_collection`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_collection "bpy.types.SpaceProperties.show_properties_collection")

  * [`bpy.types.SpaceProperties.show_properties_constraints`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_constraints "bpy.types.SpaceProperties.show_properties_constraints")

  * [`bpy.types.SpaceProperties.show_properties_data`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_data "bpy.types.SpaceProperties.show_properties_data")

  * [`bpy.types.SpaceProperties.show_properties_effects`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_effects "bpy.types.SpaceProperties.show_properties_effects")

  * [`bpy.types.SpaceProperties.show_properties_material`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_material "bpy.types.SpaceProperties.show_properties_material")

  * [`bpy.types.SpaceProperties.show_properties_modifiers`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_modifiers "bpy.types.SpaceProperties.show_properties_modifiers")

  * [`bpy.types.SpaceProperties.show_properties_object`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_object "bpy.types.SpaceProperties.show_properties_object")

  * [`bpy.types.SpaceProperties.show_properties_output`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_output "bpy.types.SpaceProperties.show_properties_output")

  * [`bpy.types.SpaceProperties.show_properties_particles`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_particles "bpy.types.SpaceProperties.show_properties_particles")

  * [`bpy.types.SpaceProperties.show_properties_physics`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_physics "bpy.types.SpaceProperties.show_properties_physics")

  * [`bpy.types.SpaceProperties.show_properties_render`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_render "bpy.types.SpaceProperties.show_properties_render")

  * [`bpy.types.SpaceProperties.show_properties_scene`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_scene "bpy.types.SpaceProperties.show_properties_scene")

  * [`bpy.types.SpaceProperties.show_properties_texture`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_texture "bpy.types.SpaceProperties.show_properties_texture")

  * [`bpy.types.SpaceProperties.show_properties_tool`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_tool "bpy.types.SpaceProperties.show_properties_tool")

  * [`bpy.types.SpaceProperties.show_properties_view_layer`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_view_layer "bpy.types.SpaceProperties.show_properties_view_layer")

  * [`bpy.types.SpaceProperties.show_properties_world`](bpy.types.SpaceProperties.md#bpy.types.SpaceProperties.show_properties_world "bpy.types.SpaceProperties.show_properties_world")


### bpy.types.SpaceSequenceEditor

#### Removed

  * **show_backdrop**


### bpy.types.SpaceSpreadsheet

#### Renamed

  * **columns** -> [`bpy.types.SpaceSpreadsheet.tables`](bpy.types.SpaceSpreadsheet.md#bpy.types.SpaceSpreadsheet.tables "bpy.types.SpaceSpreadsheet.tables")

  * **display_viewer_path_collapsed** -> [`bpy.types.SpaceSpreadsheet.show_internal_attributes`](bpy.types.SpaceSpreadsheet.md#bpy.types.SpaceSpreadsheet.show_internal_attributes "bpy.types.SpaceSpreadsheet.show_internal_attributes")


### bpy.types.SpaceUVEditor

#### Added

  * [`bpy.types.SpaceUVEditor.uv_face_opacity`](bpy.types.SpaceUVEditor.md#bpy.types.SpaceUVEditor.uv_face_opacity "bpy.types.SpaceUVEditor.uv_face_opacity")


#### Renamed

  * **show_texpaint** -> [`bpy.types.SpaceUVEditor.show_uv`](bpy.types.SpaceUVEditor.md#bpy.types.SpaceUVEditor.show_uv "bpy.types.SpaceUVEditor.show_uv")


### bpy.types.Strip

#### Removed

  * **override_cache_settings**

  * **use_cache_composite**

  * **use_cache_preprocessed**

  * **use_cache_raw**


#### Function Arguments

  * [`bpy.types.Strip.split`](bpy.types.Strip.md#bpy.types.Strip.split "bpy.types.Strip.split") (frame, split_method, ignore_connections), _was (frame, split_method)_


### bpy.types.StripsMeta

#### Function Arguments

  * [`bpy.types.StripsMeta.new_effect`](bpy.types.StripsMeta.md#bpy.types.StripsMeta.new_effect "bpy.types.StripsMeta.new_effect") (name, type, channel, frame_start, frame_end, input1, input2), _was (name, type, channel, frame_start, frame_end, seq1, seq2)_


### bpy.types.StripsTopLevel

#### Function Arguments

  * [`bpy.types.StripsTopLevel.new_effect`](bpy.types.StripsTopLevel.md#bpy.types.StripsTopLevel.new_effect "bpy.types.StripsTopLevel.new_effect") (name, type, channel, frame_start, frame_end, input1, input2), _was (name, type, channel, frame_start, frame_end, seq1, seq2)_


### bpy.types.SubsurfModifier

#### Added

  * [`bpy.types.SubsurfModifier.open_adaptive_subdivision_panel`](bpy.types.SubsurfModifier.md#bpy.types.SubsurfModifier.open_adaptive_subdivision_panel "bpy.types.SubsurfModifier.open_adaptive_subdivision_panel")

  * [`bpy.types.SubsurfModifier.open_advanced_panel`](bpy.types.SubsurfModifier.md#bpy.types.SubsurfModifier.open_advanced_panel "bpy.types.SubsurfModifier.open_advanced_panel")


### bpy.types.ThemeClipEditor

#### Added

  * [`bpy.types.ThemeClipEditor.preview_range`](bpy.types.ThemeClipEditor.md#bpy.types.ThemeClipEditor.preview_range "bpy.types.ThemeClipEditor.preview_range")


### bpy.types.ThemeInfo

#### Removed

  * **info_error**

  * **info_info**

  * **info_warning**


### bpy.types.ThemeNodeEditor

#### Added

  * [`bpy.types.ThemeNodeEditor.closure_zone`](bpy.types.ThemeNodeEditor.md#bpy.types.ThemeNodeEditor.closure_zone "bpy.types.ThemeNodeEditor.closure_zone")


### bpy.types.ThemeWidgetStateColors

#### Added

  * [`bpy.types.ThemeWidgetStateColors.error`](bpy.types.ThemeWidgetStateColors.md#bpy.types.ThemeWidgetStateColors.error "bpy.types.ThemeWidgetStateColors.error")

  * [`bpy.types.ThemeWidgetStateColors.info`](bpy.types.ThemeWidgetStateColors.md#bpy.types.ThemeWidgetStateColors.info "bpy.types.ThemeWidgetStateColors.info")

  * [`bpy.types.ThemeWidgetStateColors.success`](bpy.types.ThemeWidgetStateColors.md#bpy.types.ThemeWidgetStateColors.success "bpy.types.ThemeWidgetStateColors.success")

  * [`bpy.types.ThemeWidgetStateColors.warning`](bpy.types.ThemeWidgetStateColors.md#bpy.types.ThemeWidgetStateColors.warning "bpy.types.ThemeWidgetStateColors.warning")


### bpy.types.ToolSettings

#### Added

  * [`bpy.types.ToolSettings.playhead_snap_distance`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.playhead_snap_distance "bpy.types.ToolSettings.playhead_snap_distance")

  * [`bpy.types.ToolSettings.snap_playhead_element`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.snap_playhead_element "bpy.types.ToolSettings.snap_playhead_element")

  * [`bpy.types.ToolSettings.snap_playhead_frame_step`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.snap_playhead_frame_step "bpy.types.ToolSettings.snap_playhead_frame_step")

  * [`bpy.types.ToolSettings.snap_playhead_second_step`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.snap_playhead_second_step "bpy.types.ToolSettings.snap_playhead_second_step")

  * [`bpy.types.ToolSettings.use_snap_driver`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.use_snap_driver "bpy.types.ToolSettings.use_snap_driver")

  * [`bpy.types.ToolSettings.use_snap_driver_absolute`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.use_snap_driver_absolute "bpy.types.ToolSettings.use_snap_driver_absolute")

  * [`bpy.types.ToolSettings.use_snap_playhead`](bpy.types.ToolSettings.md#bpy.types.ToolSettings.use_snap_playhead "bpy.types.ToolSettings.use_snap_playhead")


### bpy.types.UIList

#### Added

  * [`bpy.types.UIList.bitflag_item_never_show`](bpy.types.UIList.md#bpy.types.UIList.bitflag_item_never_show "bpy.types.UIList.bitflag_item_never_show")


### bpy.types.USERPREF_UL_asset_libraries

#### Function Arguments

  * [`bpy.types.USERPREF_UL_asset_libraries.draw_item`](bpy.types.USERPREF_UL_asset_libraries.md#bpy.types.USERPREF_UL_asset_libraries.draw_item "bpy.types.USERPREF_UL_asset_libraries.draw_item") (self, _context, layout, _data, item, _icon, _active_data, _active_propname, _index), _was (self, _context, layout, _data, item, icon, _active_data, _active_propname, _index)_


### bpy.types.UnifiedPaintSettings

#### Added

  * [`bpy.types.UnifiedPaintSettings.hue_jitter`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.hue_jitter "bpy.types.UnifiedPaintSettings.hue_jitter")

  * [`bpy.types.UnifiedPaintSettings.saturation_jitter`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.saturation_jitter "bpy.types.UnifiedPaintSettings.saturation_jitter")

  * [`bpy.types.UnifiedPaintSettings.use_color_jitter`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_color_jitter "bpy.types.UnifiedPaintSettings.use_color_jitter")

  * [`bpy.types.UnifiedPaintSettings.use_random_press_hue`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_random_press_hue "bpy.types.UnifiedPaintSettings.use_random_press_hue")

  * [`bpy.types.UnifiedPaintSettings.use_random_press_sat`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_random_press_sat "bpy.types.UnifiedPaintSettings.use_random_press_sat")

  * [`bpy.types.UnifiedPaintSettings.use_random_press_val`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_random_press_val "bpy.types.UnifiedPaintSettings.use_random_press_val")

  * [`bpy.types.UnifiedPaintSettings.use_stroke_random_hue`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_stroke_random_hue "bpy.types.UnifiedPaintSettings.use_stroke_random_hue")

  * [`bpy.types.UnifiedPaintSettings.use_stroke_random_sat`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_stroke_random_sat "bpy.types.UnifiedPaintSettings.use_stroke_random_sat")

  * [`bpy.types.UnifiedPaintSettings.use_stroke_random_val`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.use_stroke_random_val "bpy.types.UnifiedPaintSettings.use_stroke_random_val")

  * [`bpy.types.UnifiedPaintSettings.value_jitter`](bpy.types.UnifiedPaintSettings.md#bpy.types.UnifiedPaintSettings.value_jitter "bpy.types.UnifiedPaintSettings.value_jitter")


### bpy.types.View3DOverlay

#### Added

  * [`bpy.types.View3DOverlay.use_gpencil_onion_skin_active_object`](bpy.types.View3DOverlay.md#bpy.types.View3DOverlay.use_gpencil_onion_skin_active_object "bpy.types.View3DOverlay.use_gpencil_onion_skin_active_object")


### bpy.types.ViewLayer

#### Added

  * [`bpy.types.ViewLayer.use_grease_pencil`](bpy.types.ViewLayer.md#bpy.types.ViewLayer.use_grease_pencil "bpy.types.ViewLayer.use_grease_pencil")

  * [`bpy.types.ViewLayer.use_pass_grease_pencil`](bpy.types.ViewLayer.md#bpy.types.ViewLayer.use_pass_grease_pencil "bpy.types.ViewLayer.use_pass_grease_pencil")


### bpy.types.Window

#### Function Arguments

  * [`bpy.types.Window.event_simulate`](bpy.types.Window.md#bpy.types.Window.event_simulate "bpy.types.Window.event_simulate") (type, value, unicode, x, y, shift, ctrl, alt, oskey, hyper), _was (type, value, unicode, x, y, shift, ctrl, alt, oskey)_
