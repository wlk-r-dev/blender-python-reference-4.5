# Image Buffer Types (imbuf.types)

This module provides access to image buffer types.

Note

Image buffer is also the structure used by [`bpy.types.Image`](bpy.types.Image.html#bpy.types.Image "bpy.types.Image") ID type to store and manipulate image data at runtime.

_class _imbuf.types.ImBuf
    

copy()
    

Returns:
    

A copy of the image.

Return type:
    

`ImBuf`

crop(_min_ , _max_)
    

Crop the image.

Parameters:
    

  * **min** (_tuple_ _[__int_ _,__int_ _]_) – X, Y minimum.

  * **max** (_tuple_ _[__int_ _,__int_ _]_) – X, Y maximum.


free()
    

Clear image data immediately (causing an error on re-use).

resize(_size_ , _method ='FAST'_)
    

Resize the image.

Parameters:
    

  * **size** (_tuple_ _[__int_ _,__int_ _]_) – New size.

  * **method** (_str_) – Method of resizing (‘FAST’, ‘BILINEAR’)


channels
    

Number of bit-planes.

Type:
    

int

filepath
    

filepath associated with this image.

Type:
    

str

planes
    

Number of bits associated with this image.

Type:
    

int

ppm
    

pixels per meter.

Type:
    

pair of floats

size
    

size of the image in pixels.

Type:
    

pair of ints
