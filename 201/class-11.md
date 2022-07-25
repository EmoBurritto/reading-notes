# Audio, Video, Images

## Video and Audio Content

plugin-based, properietary, technologies like Flash were used to handle audio and video files, now obsolete 

HTML5 allowed video and audio elements 

container formats- MP3, MP4 and WebM; define structure of media file 

A WebM container typically packages Vorbis or Opus audio with VP8/VP9 video. This is supported in all modern browsers, though older versions may not work.

An MP4 container often packages AAC or MP3 audio with H.264 video. This is also supported in all modern browsers, as well as Internet Explorer.

The Ogg container tends to use Vorbis audio and Theora video. This is best supported in Firefox and Chrome, but has basically been superseded by the better quality WebM format.


(reference: https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

## Questions 

1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.

plugin-based, properietary, technologies like Flash were used to handle audio and video files, now obsolete 

2. Describe the use of the src and controls attributes in the <video> element.

src- is the path given from HTML to audio or video file 

control- allows the user control with audio or visual file with at minmimum; start, stop and adjust volume 

3. Why is it important to have fallback content inside the <video> element?

in order for user with older web interface have access to pathway to media file 

4. Write a very short story where <audio> and <video> are characters.

Audo and Video elements are like the new kids in the block when it comes to HTML. They need a src and control to allow user friendliness with others so they can be fully understood. They are now supported by the community. 

## A Complete Guide To Grid

CSS Grid Layout (aka “Grid” or “CSS Grid”), is a two-dimensional grid-based layout system that, compared to any web layout system of the past, completely changes the way we design user interfaces. CSS has always been used to layout our web pages, but it’s never done a very good job of it. First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance). Flexbox is also a very great layout tool, but its one-directional flow has different use cases — and they actually work together quite well! Grid is the very first CSS module created specifically to solve the layout problems we’ve all been hacking our way around for as long as we’ve been making websites.

(reference: https://css-tricks.com/snippets/css/complete-guide-grid/)

## Questions 

1. How does Grid layout differ from Flex?

Flex is one-directional flow. 

Grid is two-dimensional flow. 

2. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

grid container- direct parent of grid item 

grid item- children of grid container; nested elements are not grid items 

grid line- dividing lines othat make up structure of grid; can be vertical, column grid lines, or horizontal, row grid lines. 

## Responsive Images

srcset:

An image filename (elva-fairy-480w.jpg)

A space

The image's intrinsic width in pixels (480w) — note that this uses the w unit, not px as you might expect. An image's intrinsic size is its real size, which can be found by inspecting the image file on your computer (for example, on a Mac you can select the image in Finder and press Cmd + I to bring up the info screen).

sizes: 

A media condition ((max-width:600px)) — you'll learn more about these in the CSS topic, but for now let's just say that a media condition describes a possible state that the screen can be in. In this case, we are saying "when the viewport width is 600 pixels or less".

A space
The width of the slot the image will fill when the media condition is true (480px)1

Reason to use srcset and size:

Look at its device width.
Work out which media condition in the sizes list is the first one to be true.

Look at the slot size given to that media query.

Load the image referenced in the srcset list that has the same size as the slot or, if there isn't one, the first image that is bigger than the chosen slot size.

(reference:https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images )

## Questions 

1. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

In order to set the tone and size for a site regardless or medium being used to acces site; laptops, phone, tablet, etc.

2. Define the following <img> attributes srcset and sizes. Write an example of how they are used.

srcet- gives the browser a min and max value for image file to be rendered 

sizes- sets media condition for browser to chose image size to be rendered

3. How is srcset more helpful for responsive images than CSS or JavaScript?

src set allows the browser to succesfully chose right dimensions for browser support; the browser won't be pushed past it; limits and won't compress the imagew file viewability to the user

## Things I want to know more about
- using subtitles for videos that dont already have so 
- for people that are impaired or native to other language how to add to media file friendliness 
- is there standard CSS rules for video and audio elements 
- when to use grid 
