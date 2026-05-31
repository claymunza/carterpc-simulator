# carterpc-simulator
CarterPCs simulator

First, a random screenshot of Carter's face was taken and then sent to Gemini 3.5 Flash via NanoBanana with this prompt:
```
provide a vectorized flat artistic rendition of a standard front-facing view of me by keeping same hairstyle, skin tones, colors, clothing, and a single-color background
```
and then split into layers via [SeeThrough AI](https://huggingface.co/spaces/24yearsold/see-through-demo).

Prompts used on Gemini 3.1 Pro (in chronological order):

```
provide code for static HTML, CSS, JS website minimal code required to obtain this exact layout on desktop and equivalent mobile UI UX for this kind of YouTube shorts/reels interface. Put placeholders for the texts. Use exact icons and fonts. The video region should be a frame for adding other visual elements in it later.
```
```
these images are all same size and they will be placed as layers overlapping one another. First, neck then ears, then head, then hair. And this whole setup will be placed inside the video region and will have some slight motion for 4 images like a parallax idle animation. Show me what to modify and where for editing/modifying the code in index.html. Assume the 4 images are stored as /image.webp filenames
```
```
okay this is supposed to be a CarterPCs simulator. CarterPCs is a famous YouTuber. This project is an ode to gift him on his birthday. There should be some buttons and sliders on the vast empty space on the top-left corner for desktop view. On mobile view, urge the user to rotate the device to a landscape view. The buttons and sliders would change the video title and also simulate some subtitles on the video region. Right now, some placeholder text is there which needs to be removed and replaced in real-time with the new selections.
e.g. suppose a user selects video topic as "Linux", then video tone "Humorous", and selects a pre-built-in video subtopic from a range of possibilities, e.g. "switch to Linux", and then "For" from "For/Against" and now the video title would change to "Why I choose to switch to Linux" and the video subtitles would show some sample words and texts just like a real video. Let there be about 5 topics, 4 tones, and 5 subtopics, with 2 variations for for/against. That means there should be a 5*4*5*2 data structure JSON for all possible video titles and subtitles. Video content should be about 15-30 seconds (simulated via the subtitles and intense head animations). Now show me what to modify and where to modify in order to achieve all of these.
```
