# EWA Resampling for VapourSynth

Naive and unusably slow implementation of EWA Lanczos for VS. Even nnedi runs faster, so there should never by any point in using this, especially considering how small (basically unnoticeable) the quality difference to regular Lanczos is (of course, that may just be due to an implementation error, seeing as I had to guess most of the algorithm, but the outout is near-identical to ImageMagick’s, so it can’t be completely wrong). 

```py
up = core.ewa.Lanczos(clip clip, int width, int height, float radius, float blur)
```

``clip`` needs to be 16 bits.
