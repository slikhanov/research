# Screen Space Local Reflections

I'm working on this task in a background and got some acceptable results. There are still things I want to do. This page has all my best findings on the topic.

## GitHub page that inspired me to publish my researches as Markdown pages
https://github.com/variablestudio/var-research/blob/fec0514203b39a607a76b87a4e236fc1be47d68a/graphics/ssr/README.md

This is basically collection of SSLR related articles. I will probably have some duplicates on this page too.

## Screen Space Planar Reflections in Ghost Recon Wildlands
http://remi-genin.fr/blog/screen-space-plane-indexed-reflection-in-ghost-recon-wildlands/

![](http://remi-genin.fr/blog/wp-content/uploads/Motivation3.jpg)

SSR are expected to be less expensive than actual reflection rendering and more accurate than cubemap-based reflections, as long as the reflection source is present on the screen.

In controlled situations flaws can be alleviated and SSR can deliver astonishing results.

- clearly written article with code examples
- how to resolve common problems

## Optimized pixel-projected reflections for planar reflectors
[Link to PowerPoint presentation](http://advances.realtimerendering.com/s2017/PixelProjectedReflectionsAC_v_1.92.pptx)
- constrained form of SSR
- reverse the reflection tracing
- calculate which pixel is hit in the reflection, resolve later without searching
- can be selectively used where applicable
- normal maps can be approximated, but more costly
- shader code example

## Notes On Screen Space HIZ Tracing
http://bitsquid.blogspot.co.uk/2017/08/notes-on-screen-space-hiz-tracing.html

![](https://github.com/greje656/Questions/raw/master/images/ssr6.jpg)

This is the article that I want check the most.

## Upscaling half resolution screen space effects
https://tuxedolabs.blogspot.ca/2017/11/upscaling-half-resolution-screen-space.html?m=1

Congratulations, you just saved ~75% processing time for your diffuse lighting. However, there are artifacts, 
as always. But I found the results to be acceptable in most situations. Computing diffuse lighting in half 
resolution (quarter pixel count) allowed me to do eight samples per pixel instead of two, resulting in more 
accurate lighting and less noise.

## Screen Space Local Reflections v2
https://www.panda3d.org/forums/viewtopic.php?f=8&t=15742

![](http://panda3d.org.ru/_fr/2/7894072.jpg)




