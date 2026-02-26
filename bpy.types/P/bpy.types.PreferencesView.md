# PreferencesView(bpy_struct)

base class — [[bpy_struct]]

_class _bpy.types.PreferencesView(_bpy_struct_)
    

Preferences related to viewing data

border_width
    

Size of the padding around each editor.

Type:
    

int in [1, 10], default 2

color_picker_type
    

Different styles of displaying the color picker widget

  * `CIRCLE_HSV` Circle (HSV) – A circular Hue/Saturation color wheel, with Value slider.

  * `CIRCLE_HSL` Circle (HSL) – A circular Hue/Saturation color wheel, with Lightness slider.

  * `SQUARE_SV` Square (SV + H) – A square showing Saturation/Value, with Hue slider.

  * `SQUARE_HS` Square (HS + V) – A square showing Hue/Saturation, with Value slider.

  * `SQUARE_HV` Square (HV + S) – A square showing Hue/Value, with Saturation slider.


Type:
    

enum in [`'CIRCLE_HSV'`, `'CIRCLE_HSL'`, `'SQUARE_SV'`, `'SQUARE_HS'`, `'SQUARE_HV'`], default `'CIRCLE_HSV'`

factor_display_type
    

How factor values are displayed

  * `FACTOR` Factor – Display factors as values between 0 and 1.

  * `PERCENTAGE` Percentage – Display factors as percentages.


Type:
    

enum in [`'FACTOR'`, `'PERCENTAGE'`], default `'FACTOR'`

filebrowser_display_type
    

Default location where the File Editor will be displayed in

  * `SCREEN` Maximized Area – Open the temporary editor in a maximized screen.

  * `WINDOW` New Window – Open the temporary editor in a new window.


Type:
    

enum in [`'SCREEN'`, `'WINDOW'`], default `'WINDOW'`

font_path_ui
    

Path to interface font

Type:
    

string, default “”, (never None)

font_path_ui_mono
    

Path to interface monospaced Font

Type:
    

string, default “”, (never None)

gizmo_size
    

Diameter of the gizmo

Type:
    

int in [10, 200], default 75

gizmo_size_navigate_v3d
    

The Navigate Gizmo size

Type:
    

int in [30, 200], default 80

header_align
    

Default header position for new space-types

  * `NONE` Keep Existing – Keep existing header alignment.

  * `TOP` Top – Top aligned on load.

  * `BOTTOM` Bottom – Bottom align on load (except for property editors).


Type:
    

enum in [`'NONE'`, `'TOP'`, `'BOTTOM'`], default `'NONE'`

language
    

Language used for translation

  * `DEFAULT` Automatic (Automatic) – Automatically choose the system-defined language if available, or fall-back to English (US).


Type:
    

enum in [`'DEFAULT'`], default `'DEFAULT'`

lookdev_sphere_size
    

Diameter of the HDRI preview spheres

Type:
    

int in [50, 400], default 150

mini_axis_brightness
    

Brightness of the icon

Type:
    

int in [0, 10], default 8

mini_axis_size
    

The axes icon’s size

Type:
    

int in [10, 64], default 25

mini_axis_type
    

Show small rotating 3D axes in the top right corner of the 3D viewport

Type:
    

enum in [`'NONE'`, `'MINIMAL'`, `'GIZMO'`], default `'GIZMO'`

open_sublevel_delay
    

Time delay in 1/10 seconds before automatically opening sub level menus

Type:
    

int in [1, 40], default 2

open_toplevel_delay
    

Time delay in 1/10 seconds before automatically opening top level menus

Type:
    

int in [1, 40], default 5

pie_animation_timeout
    

Time needed to fully animate the pie to unfolded state (in 1/100ths of sec)

Type:
    

int in [0, 1000], default 6

pie_initial_timeout
    

Pie menus will use the initial mouse position as center for this amount of time (in 1/100ths of sec)

Type:
    

int in [0, 1000], default 0

pie_menu_confirm
    

Distance threshold after which selection is made (zero to disable)

Type:
    

int in [0, 1000], default 0

pie_menu_radius
    

Pie menu size in pixels

Type:
    

int in [0, 1000], default 100

pie_menu_threshold
    

Distance from center needed before a selection can be made

Type:
    

int in [0, 1000], default 12

pie_tap_timeout
    

Pie menu button held longer than this will dismiss menu on release (in 1/100ths of sec)

Type:
    

int in [0, 1000], default 20

playback_fps_samples
    

The number of frames to use for calculating FPS average. Zero to calculate this automatically, where the number of samples matches the target FPS.

Type:
    

int in [0, 5000], default 8

render_display_type
    

Default location where rendered images will be displayed in

  * `NONE` Keep User Interface – Images are rendered without changing the user interface.

  * `SCREEN` Maximized Area – Images are rendered in a maximized Image Editor.

  * `AREA` Image Editor – Images are rendered in an Image Editor.

  * `WINDOW` New Window – Images are rendered in a new window.


Type:
    

enum in [`'NONE'`, `'SCREEN'`, `'AREA'`, `'WINDOW'`], default `'WINDOW'`

rotation_angle
    

Rotation step for numerical pad keys (2 4 6 8)

Type:
    

float in [0, 90], default 15.0

show_addons_enabled_only
    

Only show enabled add-ons. Un-check to see all installed add-ons.

Type:
    

boolean, default False

show_column_layout
    

Use a column layout for toolbox

Type:
    

boolean, default True

show_developer_ui
    

Display advanced settings and tools for developers

Type:
    

boolean, default False

show_extensions_updates
    

Show Extensions Update Count

Type:
    

boolean, default True

show_gizmo
    

Use transform gizmos by default

Type:
    

boolean, default True

show_navigate_ui
    

Show navigation controls in 2D and 3D views which do not have scroll bars

Type:
    

boolean, default True

show_object_info
    

Include the name of the active object and the current frame number in the text info overlay

Type:
    

boolean, default True

show_playback_fps
    

Include the number of frames displayed per second in the text info overlay while animation is played back

Type:
    

boolean, default True

show_splash
    

Display splash screen on startup

Type:
    

boolean, default True

show_statusbar_memory
    

Show Blender memory usage

Type:
    

boolean, default False

show_statusbar_scene_duration
    

Show scene duration

Type:
    

boolean, default False

show_statusbar_stats
    

Show scene statistics

Type:
    

boolean, default False

show_statusbar_version
    

Show Blender version string

Type:
    

boolean, default True

show_statusbar_vram
    

Show GPU video memory usage

Type:
    

boolean, default False

show_tooltips
    

Display tooltips (when disabled, hold Alt to force display)

Type:
    

boolean, default True

show_tooltips_python
    

Show Python references in tooltips

Type:
    

boolean, default False

show_view_name
    

Include the name of the view orientation in the text info overlay

Type:
    

boolean, default True

smooth_view
    

Time to animate the view in milliseconds, zero to disable

Type:
    

int in [0, 1000], default 200

text_hinting
    

Method for making user interface text render sharp

Type:
    

enum in [`'AUTO'`, `'NONE'`, `'SLIGHT'`, `'FULL'`], default `'AUTO'`

timecode_style
    

Format of timecode displayed when not displaying timing in terms of frames

  * `MINIMAL` Minimal Info – Most compact representation, uses ‘+’ as separator for sub-second frame numbers, with left and right truncation of the timecode as necessary.

  * `SMPTE` SMPTE (Full) – Full SMPTE timecode (format is HH:MM:SS:FF).

  * `SMPTE_COMPACT` SMPTE (Compact) – SMPTE timecode showing minutes, seconds, and frames only - hours are also shown if necessary, but not by default.

  * `MILLISECONDS` Compact with Decimals – Similar to SMPTE (Compact), except that the decimal part of the second is shown instead of frames.

  * `SECONDS_ONLY` Only Seconds – Direct conversion of frame numbers to seconds.


Type:
    

enum in [`'MINIMAL'`, `'SMPTE'`, `'SMPTE_COMPACT'`, `'MILLISECONDS'`, `'SECONDS_ONLY'`], default `'MINIMAL'`

ui_line_width
    

Changes the thickness of widget outlines, lines and dots in the interface

  * `THIN` Thin – Thinner lines than the default.

  * `AUTO` Default – Automatic line width based on UI scale.

  * `THICK` Thick – Thicker lines than the default.


Type:
    

enum in [`'THIN'`, `'AUTO'`, `'THICK'`], default `'AUTO'`

ui_scale
    

Changes the size of the fonts and widgets in the interface

Type:
    

float in [0.5, 6], default 1.0

use_filter_brushes_by_tool
    

Only show brushes applicable for the currently active tool in the asset shelf. Stored in the Preferences, which may have to be saved manually if Auto-Save Preferences is disabled

Type:
    

boolean, default False

use_fresnel_edit
    

Enable a fresnel effect on edit mesh overlays. It improves shape readability of very dense meshes, but increases eye fatigue when modeling lower poly

Type:
    

boolean, default False

use_mouse_over_open
    

Open menu buttons and pull-downs automatically when the mouse is hovering

Type:
    

boolean, default False

use_save_prompt
    

Ask for confirmation when quitting with unsaved changes

Type:
    

boolean, default True

use_text_antialiasing
    

Smooth jagged edges of user interface text

Type:
    

boolean, default True

use_text_render_subpixelaa
    

Render text for optimal horizontal placement

Type:
    

boolean, default False

use_translate_interface
    

Translate all labels in menus, buttons and panels (note that this might make it hard to follow tutorials or the manual)

Type:
    

boolean, default True

use_translate_new_dataname
    

Translate the names of new data-blocks (objects, materials…)

Type:
    

boolean, default True

use_translate_reports
    

Translate additional information, such as error messages

Type:
    

boolean, default True

use_translate_tooltips
    

Translate the descriptions when hovering UI elements (recommended)

Type:
    

boolean, default True

use_weight_color_range
    

Enable color range used for weight visualization in weight painting mode

Type:
    

boolean, default False

view2d_grid_spacing_min
    

Minimum number of pixels between each gridline in 2D Viewports

Type:
    

int in [1, 500], default 45

view_frame_keyframes
    

Keyframes around cursor that we zoom around

Type:
    

int in [1, 500], default 0

view_frame_seconds
    

Seconds around cursor that we zoom around

Type:
    

float in [0, 10000], default 0.0

view_frame_type
    

How zooming to frame focuses around current frame

Type:
    

enum in [`'KEEP_RANGE'`, `'SECONDS'`, `'KEYFRAMES'`], default `'KEEP_RANGE'`

weight_color_range
    

Color range used for weight visualization in weight painting mode

Type:
    

[[ColorRamp]], (readonly, never None)

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

| 


  
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

| 

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

  
---|---  
  
## References

  * [[Preferences.view]]

| 


  
---|---
