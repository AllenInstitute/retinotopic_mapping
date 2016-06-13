#retinotopic_mapping package  

by Jun Zhuang, 2016 @ AIBS
junz AT alleninstitute DOT org  

This package contains a code base for visual area auto-segmentation of mouse visual cortex by doing 
visual sign map analysis from retinotopic maps. This analysis routine was modified from Garrett et al.,
2014 (1), which was inspired by the earlier work in primate visual system (4, 5). 


The analysis takes visual altitude and azimuth maps of mouse cortex as inputs, calculates the visual 
sign of each pixel and auto-segments the cortical surface into primary visual cortex and multiple higher
visual cortices. Ideally, the visual altitude and azimuth maps can be generated by fourier analysis of
population cortical responses to periodic sweeping checker board visual stimuli (2, 3). The code of visual 
stimulation and altitude/azimuth retinotopic map generation is not included in this package.

The package also provides some useful plotting functions to visualize the results.

Please check the jupyter notebook in the '\examples' folder for the usage.
https://github.com/zhuangjun1981/retinotopic_mapping/blob/master/retinotopic_mapping/examples/retinotopic_mapping_example.html


####Language:

1. python 2.7


####Install:
`cd <package_path>`
`python setup.py install`


####Dependencies:

1. numpy, version 1.10.4 
2. scipy, version 0.17.0
3. OpenCV-Python, version 2.4.8
4. scikit-image, version 0.12.3
5. matplotlib, version 1.5.1
6. tifffile, version 0.7.0


####Reference:

1. Garrett ME, Nauhaus I, Marshel JH, Callaway EM (2014) Topography and areal organization of mouse visual cortex. J Neurosci 34:12587-12600.

2. Kalatsky VA, Stryker MP (2003) New paradigm for optical imaging: temporally encoded maps of intrinsic signal. Neuron 38:529-545.

3. Marshel JH, Kaye AP, Nauhaus I, Callaway EM (2012) Anterior-posterior direction opponency in the superficial mouse lateral geniculate nucleus. Neuron 76:713-720.

4. Sereno MI, Dale AM, Reppas JB, Kwong KK, Belliveau JW, Brady TJ, Rosen BR, Tootell RB (1995) Borders of multiple visual areas in humans revealed by functional magnetic resonance imaging. Science 268:889-893.

5. Sereno MI, McDonald CT, Allman JM (1994) Analysis of retinotopic maps in extrastriate cortex. Cereb Cortex 4:601-620.


####Issues:

1. Most image analysis parameters are defined as number of pixels, not microns.
2. Works in windows, but not fully tested on Mac and Linux.