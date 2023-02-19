# Reading notes for Visual/Audio content, Grid, Responsive images

## Video and Audio content
- [Video and Audio](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)
1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.
In the early 2000s a Flash or Silverlight plug-in was required to run video/audio, now these are obsolete. HTML and JavaScript APIs can now do so while being more secure and most video/audio applications can render without consuming a large amount of bandwith.

2. Describe the use of the src and controls attributes in the <video> element.
`src` in the video element acts the same way as an image element- it provides a path for the source that is embedded. `controls` provides users with the ability to start/stop and control volume of the media.

3. Why is it important to have fallback content inside the <video> element?
Some browsers dont support the `video` element so it provides a way for users to view the content, usually with a link to the video file.

4. Write a very short story where <audio> and <video> are characters.
Video was a bright exuberant child always wanting to show you something but unfortunately sometimes he was too loud or too quiet or just wouldn't speak. The child video came across a humble animal named audio. Audio and video became best friends and as their friendship grew, audio would help video find the right volume and even offered control of how loud they could be.

## Grid
- [Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
1. How does Grid layout differ from Flex?
Grid is a 2D based layout system where Flex is a one directional flow with different use cases.

2. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.
- Grid container: the element where `display` is applied, it is the parent of all the grid items and container is where they live.
- Grid item: Direct descendants of the grid container
- Grid line: the dividing lines that provide the structure of the grid, can be horizontal or vertical and reside on either row or column side.

## Responsive images
- [Responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
1. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?
Not all viewports are the same dimensions so it helps prevent content from being cut off

2. Define the following `<img>` attributes `srcset` and `sizes`. Write an example of how they are used.
- `img` points to the source file, used for holding all aspects of the image you want displayed
- `srcset` lets the browser choose between a set of images, used for determining the correct image to be displayed on the viewport
- `sizes` defines media conditions and allows the best image to be chosen when media conditions are true, used for providing dimensions for the device to determine between the options which is best for application
3. How is `srcset` more helpful for responsive images than CSS or JavaScript?
It gives options rather than determining what the sizes will be so that the best possible choice for an image can be displayed without cutting off content.


## Things I want to know more about

iframes and best embedding practices for other documents
[other embedding technologies](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Other_embedding_technologies)