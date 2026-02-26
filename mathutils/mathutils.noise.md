# Noise Utilities (mathutils.noise)

The Blender noise module

mathutils.noise.cell(_position_)
    

Returns cell noise value at the specified position.

Parameters:
    

**position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

Returns:
    

The cell noise value.

Return type:
    

float

mathutils.noise.cell_vector(_position_)
    

Returns cell noise vector at the specified position.

Parameters:
    

**position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

Returns:
    

The cell noise vector.

Return type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")

mathutils.noise.fractal(_position_ , _H_ , _lacunarity_ , _octaves_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns the fractal Brownian motion (fBm) noise value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **H** (_float_) – The fractal increment factor.

  * **lacunarity** (_float_) – The gap between successive frequencies.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The fractal Brownian motion noise value.

Return type:
    

float

mathutils.noise.hetero_terrain(_position_ , _H_ , _lacunarity_ , _octaves_ , _offset_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns the heterogeneous terrain value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **H** (_float_) – The fractal dimension of the roughest areas.

  * **lacunarity** (_float_) – The gap between successive frequencies.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **offset** (_float_) – The height of the terrain above ‘sea level’.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The heterogeneous terrain value.

Return type:
    

float

mathutils.noise.hybrid_multi_fractal(_position_ , _H_ , _lacunarity_ , _octaves_ , _offset_ , _gain_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns hybrid multifractal value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **H** (_float_) – The fractal dimension of the roughest areas.

  * **lacunarity** (_float_) – The gap between successive frequencies.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **offset** (_float_) – The height of the terrain above ‘sea level’.

  * **gain** (_float_) – Scaling applied to the values.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The hybrid multifractal value.

Return type:
    

float

mathutils.noise.multi_fractal(_position_ , _H_ , _lacunarity_ , _octaves_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns multifractal noise value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **H** (_float_) – The fractal increment factor.

  * **lacunarity** (_float_) – The gap between successive frequencies.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The multifractal noise value.

Return type:
    

float

mathutils.noise.noise(_position_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns noise value from the noise basis at the position specified.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The noise value.

Return type:
    

float

mathutils.noise.noise_vector(_position_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns the noise vector from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The noise vector.

Return type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")

mathutils.noise.random()
    

Returns a random number in the range [0, 1).

Returns:
    

The random number.

Return type:
    

float

mathutils.noise.random_unit_vector(_size =3_)
    

Returns a unit vector with random entries.

Parameters:
    

**size** (_int_) – The size of the vector to be produced, in the range [2, 4].

Returns:
    

The random unit vector.

Return type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")

mathutils.noise.random_vector(_size =3_)
    

Returns a vector with random entries in the range (-1, 1).

Parameters:
    

**size** (_int_) – The size of the vector to be produced.

Returns:
    

The random vector.

Return type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")

mathutils.noise.ridged_multi_fractal(_position_ , _H_ , _lacunarity_ , _octaves_ , _offset_ , _gain_ , _noise_basis ='PERLIN_ORIGINAL'_)
    

Returns ridged multifractal value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **H** (_float_) – The fractal dimension of the roughest areas.

  * **lacunarity** (_float_) – The gap between successive frequencies.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **offset** (_float_) – The height of the terrain above ‘sea level’.

  * **gain** (_float_) – Scaling applied to the values.

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The ridged multifractal value.

Return type:
    

float

mathutils.noise.seed_set(_seed_)
    

Sets the random seed used for random_unit_vector, and random.

Parameters:
    

**seed** (_int_) – Seed used for the random generator. When seed is zero, the current time will be used instead.

mathutils.noise.turbulence(_position_ , _octaves_ , _hard_ , _noise_basis ='PERLIN_ORIGINAL'_, _amplitude_scale =0.5_, _frequency_scale =2.0_)
    

Returns the turbulence value from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **hard** (_bool_) – Specifies whether returned turbulence is hard (sharp transitions) or soft (smooth transitions).

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].

  * **amplitude_scale** (_float_) – The amplitude scaling factor.

  * **frequency_scale** (_float_) – The frequency scaling factor


Returns:
    

The turbulence value.

Return type:
    

float

mathutils.noise.turbulence_vector(_position_ , _octaves_ , _hard_ , _noise_basis ='PERLIN_ORIGINAL'_, _amplitude_scale =0.5_, _frequency_scale =2.0_)
    

Returns the turbulence vector from the noise basis at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **octaves** (_int_) – The number of different noise frequencies used.

  * **hard** (_bool_) – Specifies whether returned turbulence is hard (sharp transitions) or soft (smooth transitions).

  * **noise_basis** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].

  * **amplitude_scale** (_float_) – The amplitude scaling factor.

  * **frequency_scale** (_float_) – The frequency scaling factor


Returns:
    

The turbulence vector.

Return type:
    

[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")

mathutils.noise.variable_lacunarity(_position_ , _distortion_ , _noise_type1 ='PERLIN_ORIGINAL'_, _noise_type2 ='PERLIN_ORIGINAL'_)
    

Returns variable lacunarity noise value, a distorted variety of noise, from noise type 1 distorted by noise type 2 at the specified position.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **distortion** (_float_) – The amount of distortion.

  * **noise_type1** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].

  * **noise_type2** (_str_) – Enumerator in [‘BLENDER’, ‘PERLIN_ORIGINAL’, ‘PERLIN_NEW’, ‘VORONOI_F1’, ‘VORONOI_F2’, ‘VORONOI_F3’, ‘VORONOI_F4’, ‘VORONOI_F2F1’, ‘VORONOI_CRACKLE’, ‘CELLNOISE’].


Returns:
    

The variable lacunarity noise value.

Return type:
    

float

mathutils.noise.voronoi(_position_ , _distance_metric ='DISTANCE'_, _exponent =2.5_)
    

Returns a list of distances to the four closest features and their locations.

Parameters:
    

  * **position** ([`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")) – The position to evaluate the selected noise function.

  * **distance_metric** (_str_) – Enumerator in [‘DISTANCE’, ‘DISTANCE_SQUARED’, ‘MANHATTAN’, ‘CHEBYCHEV’, ‘MINKOVSKY’, ‘MINKOVSKY_HALF’, ‘MINKOVSKY_FOUR’].

  * **exponent** (_float_) – The exponent for Minkowski distance metric.


Returns:
    

A list of distances to the four closest features and their locations.

Return type:
    

list[list[float] | list[[`mathutils.Vector`](mathutils.md#mathutils.Vector "mathutils.Vector")]]
