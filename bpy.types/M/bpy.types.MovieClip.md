# MovieClip(ID)

base classes — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`ID`](bpy.types.ID.md#bpy.types.ID "bpy.types.ID")

_class _bpy.types.MovieClip(_ID_)
    

MovieClip data-block referencing an external movie file

animation_data
    

Animation data for this data-block

Type:
    

[`AnimData`](bpy.types.AnimData.md#bpy.types.AnimData "bpy.types.AnimData"), (readonly)

colorspace_settings
    

Input color space settings

Type:
    

[`ColorManagedInputColorspaceSettings`](bpy.types.ColorManagedInputColorspaceSettings.md#bpy.types.ColorManagedInputColorspaceSettings "bpy.types.ColorManagedInputColorspaceSettings"), (readonly)

display_aspect
    

Display Aspect for this clip, does not affect rendering

Type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector") of 2 items in [0.1, inf], default (1.0, 1.0)

filepath
    

Filename of the movie or sequence file

Type:
    

string, default “”, (never None, blend relative `//` prefix supported)

fps
    

Detected frame rate of the movie clip in frames per second

Type:
    

float in [-inf, inf], default 0.0, (readonly)

frame_duration
    

Detected duration of movie clip in frames

Type:
    

int in [-inf, inf], default 0, (readonly)

frame_offset
    

Offset of footage first frame relative to its file name (affects only how footage is loading, does not change data associated with a clip)

Type:
    

int in [-inf, inf], default 0

frame_start
    

Global scene frame number at which this movie starts playing (affects all data associated with a clip)

Type:
    

int in [-inf, inf], default 1

grease_pencil
    

Grease Pencil data for this movie clip

Type:
    

[`GreasePencil`](bpy.types.GreasePencil.md#bpy.types.GreasePencil "bpy.types.GreasePencil")

proxy
    

Type:
    

[`MovieClipProxy`](bpy.types.MovieClipProxy.md#bpy.types.MovieClipProxy "bpy.types.MovieClipProxy"), (readonly)

size
    

Width and height in pixels, zero when image data can’t be loaded

Type:
    

int array of 2 items in [-inf, inf], default (0, 0), (readonly)

source
    

Where the clip comes from

  * `SEQUENCE` Image Sequence – Multiple image files, as a sequence.

  * `MOVIE` Movie File – Movie file.


Type:
    

enum in [`'SEQUENCE'`, `'MOVIE'`], default `'SEQUENCE'`, (readonly)

tracking
    

Type:
    

[`MovieTracking`](bpy.types.MovieTracking.md#bpy.types.MovieTracking "bpy.types.MovieTracking"), (readonly)

use_proxy
    

Use a preview proxy and/or timecode index for this clip

Type:
    

boolean, default False

use_proxy_custom_directory
    

Create proxy images in a custom directory (default is movie location)

Type:
    

boolean, default False

metadata()
    

Retrieve metadata of the movie file

Returns:
    

Dict-like object containing the metadata

Return type:
    

[`IDPropertyWrapPtr`](bpy.types.IDPropertyWrapPtr.md#bpy.types.IDPropertyWrapPtr "bpy.types.IDPropertyWrapPtr")

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.md#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")
  * [`ID.name`](bpy.types.ID.md#bpy.types.ID.name "bpy.types.ID.name")
  * [`ID.name_full`](bpy.types.ID.md#bpy.types.ID.name_full "bpy.types.ID.name_full")
  * [`ID.id_type`](bpy.types.ID.md#bpy.types.ID.id_type "bpy.types.ID.id_type")
  * [`ID.session_uid`](bpy.types.ID.md#bpy.types.ID.session_uid "bpy.types.ID.session_uid")
  * [`ID.is_evaluated`](bpy.types.ID.md#bpy.types.ID.is_evaluated "bpy.types.ID.is_evaluated")
  * [`ID.original`](bpy.types.ID.md#bpy.types.ID.original "bpy.types.ID.original")
  * [`ID.users`](bpy.types.ID.md#bpy.types.ID.users "bpy.types.ID.users")
  * [`ID.use_fake_user`](bpy.types.ID.md#bpy.types.ID.use_fake_user "bpy.types.ID.use_fake_user")
  * [`ID.use_extra_user`](bpy.types.ID.md#bpy.types.ID.use_extra_user "bpy.types.ID.use_extra_user")
  * [`ID.is_embedded_data`](bpy.types.ID.md#bpy.types.ID.is_embedded_data "bpy.types.ID.is_embedded_data")

| 

  * [`ID.is_missing`](bpy.types.ID.md#bpy.types.ID.is_missing "bpy.types.ID.is_missing")
  * [`ID.is_runtime_data`](bpy.types.ID.md#bpy.types.ID.is_runtime_data "bpy.types.ID.is_runtime_data")
  * [`ID.is_editable`](bpy.types.ID.md#bpy.types.ID.is_editable "bpy.types.ID.is_editable")
  * [`ID.tag`](bpy.types.ID.md#bpy.types.ID.tag "bpy.types.ID.tag")
  * [`ID.is_library_indirect`](bpy.types.ID.md#bpy.types.ID.is_library_indirect "bpy.types.ID.is_library_indirect")
  * [`ID.library`](bpy.types.ID.md#bpy.types.ID.library "bpy.types.ID.library")
  * [`ID.library_weak_reference`](bpy.types.ID.md#bpy.types.ID.library_weak_reference "bpy.types.ID.library_weak_reference")
  * [`ID.asset_data`](bpy.types.ID.md#bpy.types.ID.asset_data "bpy.types.ID.asset_data")
  * [`ID.override_library`](bpy.types.ID.md#bpy.types.ID.override_library "bpy.types.ID.override_library")
  * [`ID.preview`](bpy.types.ID.md#bpy.types.ID.preview "bpy.types.ID.preview")

  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")

| 

  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`ID.rename`](bpy.types.ID.md#bpy.types.ID.rename "bpy.types.ID.rename")
  * [`ID.evaluated_get`](bpy.types.ID.md#bpy.types.ID.evaluated_get "bpy.types.ID.evaluated_get")
  * [`ID.copy`](bpy.types.ID.md#bpy.types.ID.copy "bpy.types.ID.copy")
  * [`ID.asset_mark`](bpy.types.ID.md#bpy.types.ID.asset_mark "bpy.types.ID.asset_mark")
  * [`ID.asset_clear`](bpy.types.ID.md#bpy.types.ID.asset_clear "bpy.types.ID.asset_clear")
  * [`ID.asset_generate_preview`](bpy.types.ID.md#bpy.types.ID.asset_generate_preview "bpy.types.ID.asset_generate_preview")
  * [`ID.override_create`](bpy.types.ID.md#bpy.types.ID.override_create "bpy.types.ID.override_create")
  * [`ID.override_hierarchy_create`](bpy.types.ID.md#bpy.types.ID.override_hierarchy_create "bpy.types.ID.override_hierarchy_create")
  * [`ID.user_clear`](bpy.types.ID.md#bpy.types.ID.user_clear "bpy.types.ID.user_clear")
  * [`ID.user_remap`](bpy.types.ID.md#bpy.types.ID.user_remap "bpy.types.ID.user_remap")
  * [`ID.make_local`](bpy.types.ID.md#bpy.types.ID.make_local "bpy.types.ID.make_local")
  * [`ID.user_of_id`](bpy.types.ID.md#bpy.types.ID.user_of_id "bpy.types.ID.user_of_id")
  * [`ID.animation_data_create`](bpy.types.ID.md#bpy.types.ID.animation_data_create "bpy.types.ID.animation_data_create")
  * [`ID.animation_data_clear`](bpy.types.ID.md#bpy.types.ID.animation_data_clear "bpy.types.ID.animation_data_clear")
  * [`ID.update_tag`](bpy.types.ID.md#bpy.types.ID.update_tag "bpy.types.ID.update_tag")
  * [`ID.preview_ensure`](bpy.types.ID.md#bpy.types.ID.preview_ensure "bpy.types.ID.preview_ensure")
  * [`ID.bl_rna_get_subclass`](bpy.types.ID.md#bpy.types.ID.bl_rna_get_subclass "bpy.types.ID.bl_rna_get_subclass")
  * [`ID.bl_rna_get_subclass_py`](bpy.types.ID.md#bpy.types.ID.bl_rna_get_subclass_py "bpy.types.ID.bl_rna_get_subclass_py")

  
---|---  
  
## References

  * [`bpy.context.edit_movieclip`](bpy.context.md#bpy.context.edit_movieclip "bpy.context.edit_movieclip")
  * [`BlendData.movieclips`](bpy.types.BlendData.md#bpy.types.BlendData.movieclips "bpy.types.BlendData.movieclips")
  * [`BlendDataMovieClips.load`](bpy.types.BlendDataMovieClips.md#bpy.types.BlendDataMovieClips.load "bpy.types.BlendDataMovieClips.load")
  * [`BlendDataMovieClips.remove`](bpy.types.BlendDataMovieClips.md#bpy.types.BlendDataMovieClips.remove "bpy.types.BlendDataMovieClips.remove")
  * [`CameraBackgroundImage.clip`](bpy.types.CameraBackgroundImage.md#bpy.types.CameraBackgroundImage.clip "bpy.types.CameraBackgroundImage.clip")
  * [`CameraSolverConstraint.clip`](bpy.types.CameraSolverConstraint.md#bpy.types.CameraSolverConstraint.clip "bpy.types.CameraSolverConstraint.clip")
  * [`CompositorNodeKeyingScreen.clip`](bpy.types.CompositorNodeKeyingScreen.md#bpy.types.CompositorNodeKeyingScreen.clip "bpy.types.CompositorNodeKeyingScreen.clip")
  * [`CompositorNodeMovieClip.clip`](bpy.types.CompositorNodeMovieClip.md#bpy.types.CompositorNodeMovieClip.clip "bpy.types.CompositorNodeMovieClip.clip")
  * [`CompositorNodeMovieDistortion.clip`](bpy.types.CompositorNodeMovieDistortion.md#bpy.types.CompositorNodeMovieDistortion.clip "bpy.types.CompositorNodeMovieDistortion.clip")
  * [`CompositorNodePlaneTrackDeform.clip`](bpy.types.CompositorNodePlaneTrackDeform.md#bpy.types.CompositorNodePlaneTrackDeform.clip "bpy.types.CompositorNodePlaneTrackDeform.clip")

| 

  * [`CompositorNodeStabilize.clip`](bpy.types.CompositorNodeStabilize.md#bpy.types.CompositorNodeStabilize.clip "bpy.types.CompositorNodeStabilize.clip")
  * [`CompositorNodeTrackPos.clip`](bpy.types.CompositorNodeTrackPos.md#bpy.types.CompositorNodeTrackPos.clip "bpy.types.CompositorNodeTrackPos.clip")
  * [`FollowTrackConstraint.clip`](bpy.types.FollowTrackConstraint.md#bpy.types.FollowTrackConstraint.clip "bpy.types.FollowTrackConstraint.clip")
  * [`MovieClipStrip.clip`](bpy.types.MovieClipStrip.md#bpy.types.MovieClipStrip.clip "bpy.types.MovieClipStrip.clip")
  * [`ObjectSolverConstraint.clip`](bpy.types.ObjectSolverConstraint.md#bpy.types.ObjectSolverConstraint.clip "bpy.types.ObjectSolverConstraint.clip")
  * [`Scene.active_clip`](bpy.types.Scene.md#bpy.types.Scene.active_clip "bpy.types.Scene.active_clip")
  * [`SpaceClipEditor.clip`](bpy.types.SpaceClipEditor.md#bpy.types.SpaceClipEditor.clip "bpy.types.SpaceClipEditor.clip")
  * [`StripsMeta.new_clip`](bpy.types.StripsMeta.md#bpy.types.StripsMeta.new_clip "bpy.types.StripsMeta.new_clip")
  * [`StripsTopLevel.new_clip`](bpy.types.StripsTopLevel.md#bpy.types.StripsTopLevel.new_clip "bpy.types.StripsTopLevel.new_clip")

  
---|---
