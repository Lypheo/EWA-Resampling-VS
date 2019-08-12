# EWA Resampling for VapourSynth

Naive and unusably slow implementation of EWA Lanczos for VS. Even nnedi runs faster, so there should never by any point in using this, especially considering how small (basically unnoticeable) the quality difference to regular Lanczos is. 

```py
up = core.ewa.Lanczos(clip clip, int width, int height, float radius, float blur)
```
