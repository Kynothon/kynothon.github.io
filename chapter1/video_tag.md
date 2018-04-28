# The Video Tag

In the dark age of video streaming, consumers will use dedicated software such as **RealNetworks** or install plugins to their web browsers a.k.a. the infamous **Flash Player**. These solutions lived during the emergence of the web as we know it.

## HTML5 `<video>` tag
Februry 28 2007, [Web Hypertext Application Technology Working Group (WHATWG)](https://whatwg.org/) mailing list a [message] (https://web.archive.org/web/20070312050749/https://lists.whatwg.org/pipermail/whatwg-whatwg.org/2007-February/009702.html) from Anne van Kesteren, describe to the world a new API that could be an equivalent to the `Audio()` object for video playback. This new `<video>` tag would be used like the `<image>` tag to reserve space on a page and behave like the `Audio()` object in term of possible actions. It was the birth of the `<video>` tag.
The same day a demo show to the world how it could look like to play video without the need of plugins in a web browser.

[![Video embedded in Opera browser alpha by Hakon Wiwm Lie](http://img.youtube.com/vi/hUqC1URVyt/0.jpg)](http://www.youtube.com/watch?v=hUqC1URVyt)

The `<video>` tag is accepted to be part of the HTML5 specification released on 28 October 2014.

## Video Formats
From the beginning the `<video>` tag was intended to make use of the good video format of the time. Picture quality, compression and low processing power were the quality the _WHATWG_ was looking for. The selected format should be royality free and be implementable in hardware. Theora video with Vorbis Audio codecs in an Ogg container were the first choice. This selections wasn't widely spread at the time, so a later revision opened the possibility to other codecs.

Beside the Theora/Vorbis in OGG container, H264/AAC in MP4 is widely supported. WebM with VP8/9 is another available format supported by Google. [3]

## Use the Video tag

```
<!DOCTYPE html>
<html>
<body>

<video width="320" height="240" controls>
  <source src="https://www.w3schools.com/TAGS/movie.mp4" type="video/mp4">
  <source src="https://www.w3schools.com/TAGS/movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>

<p><strong>Note:</strong> The video tag is not supported in Internet Explorer 8 and earlier versions.</p>

</body>
</html>
```(https://www.w3schools.com/TAGS/tag_video.asp)

## References
1. https://developer.mozilla.org/en-US/docs/Web/HTML/Element/video
2. https://html.spec.whatwg.org/multipage/media.html#the-video-element
[3]. https://developer.mozilla.org/en-US/docs/Web/HTML/Supported_media_formats