# CLFTestImage
 Test Image for CLF Evaluation and Development

Mostly a discussion point at the moment.

![](images/CLF_testImagePrototype_v008.jpg)

The ramps and the bottom shown in 3D space.
![](images/fullRangeSpikeExample_v001.png)

The intent here is to cover as much of the possible half float range, both positive and negative, using half float style quantization.

Since the fist CLF inmplementation meeting, a number of features have been added.

* Subnormal value row in the full float range ramps.
* Full range float ramps now cover full positive a negative spaces.
* Cube has been expanded to 64x64, but not covers negative space, so no precision has been gained.
* WRGBCYM 0.0 -> 1.0 ramps
* WRGBCYM 0.18 -15 to +15 stops patch ramps
* Selection of easy to sample patch squares W,R,G,B,C,M,Y,inf,-inf,nan,0,65504. (should probably be expanded on).


# 15 Sep 2021

Removed NaN and Inf example Pixels from bottom left.

# 25 Aug 2020

General script tidy up, not functional changes.
![](images/fullDAGcap.png)


# Description:

![](images/CLF_docImage_v008.jpg)

## Creations date
This section is simply a data stamp to make it easier to diferentiate versions of the image created at different times.

## Image is composed of the following subsections

## 33x33 Cubes

There are two 33x33 cubes here.
The one on the bottom runs from -1.0 to 1.0
The one on the top runs from -65504 to 65504

![](images/documentation/isolatedSection_33x33_Cubes.png)

![](images/33x33_0to1_cube.png)

![](images/33x33_0to65504_cube.png)


## Macbeth

This is a miniature Macbeth in ACES2065-1, based on the colourscience.org values

![](images/documentation/isolatedSection_macbeth.png)

## Grey Ramps

This is a set of 0 -> 1 greyscale ramps.

![](images/documentation/isolatedSection_grey_ramps.png)

Linear
* sRGB
*Gamma 2.2
*Gamma 2.4
*Gamma 2.6
*ST.2084

## Pure Ramps + Macbeth Ramps

This is a set of pure macbeth patches in 1/2 stop increments.

![](images/documentation/isolatedSection_pure_ramps_+_macbeth_ramps.png)

Each patch is 16x4 pixels, with the 1.0 patch's bottom corner starting at x=496 y=225

## Spiderweb

This is a set of Ramps designed to generate a spiderweb whe viewed on a vector scope.

![](images/documentation/isolatedsection_spiderweb.png)

![](images/Spiderweb_on_vectorscope.png)

## Extents Lattice

This section of ramps is designed to produce a bounding box around all possible normal positive and negative values when viewed in 3D.

![](images/documentation/isolatedSection_extents_latice.png)

![](images/extentsCubeVis.png)
