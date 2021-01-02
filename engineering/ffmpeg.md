# Command line FFmpeg study

## Encoding Animated GIF

Converting a video to GIF file with ffmpeg:

`ffmpeg -i input.flv -ss 00:00:00.000 -pix_fmt rgb24 -r 10 -s 320x240 -t 00:00:10.000 output.gif`

It works great, but output gif file has a very low quality.

Quality improvements:

ffmpeg can output high quality GIF. 

`ffmpeg -ss 30 -t 3 -i input.mp4 -vf "fps=10,scale=320:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 output.gif`

- This example will skip the first 30 seconds (-ss 30) of the input and create a 3 second output (-t 3).
- [fps](https://ffmpeg.org/ffmpeg-filters.html#fps) filter sets the frame rate. A rate of 10 frames per second is used in the example.
  scale filter will resize the output to 320 pixels wide and automatically determine the height while preserving 
  the aspect ratio. The lanczos scaling algorithm is used in this example.
- palettegen and paletteuse filters will generate and use a custom palette generated from your input. 
  These filters have many options, so refer to the links for a list of all available options and values. 
  Also see the Advanced options section below.
- split filter will allow everything to be done in one command and avoids having to create a temporary PNG file of the palette.
- Control looping with -loop output option but the values are confusing. A value of 0 is infinite looping, -1 is no looping, 
  and 1 will loop once meaning it will play twice. So a value of 10 will cause the GIF to play 11 times.

Advanced options

The palettegen and paletteuse filters have many additional options. The most important are:

- stats_mode (palettegen). You can force the filters to focus the palette on the general picture (full which is the default), only the moving parts (diff), or each individual frame (single). For example, to generate a palette for each individual frame use palettegen=stats_mode=single & paletteuse=new=1.
- dither (paletteuse). Choose the dithering algorithm. There are three main types: deterministic (bayer), error diffusion (all the others including the default sierra2_4a), and none. Your GIF may look better using a particular dithering algorithm, or no dithering at all. If you want to try bayer be sure to test the bayer_scale option too.
- See High quality GIF with FFmpeg for explanations, example images, and more detailed info for advanced usage.

Also see the palettegen and paletteuse documentation for all available options and values.

