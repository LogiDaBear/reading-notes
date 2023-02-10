# Reading Notes for Images, Color, Text (HTML and CSS)

## HTML Media
[UsingImagesInHTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
[CommonImageTypes](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types)
[ChoosingImageFormats](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types#choosing_an_image_format)

1. What is a real world use case for the alt attribute being used in a website?

If you lived out in BFE you could have an alt tag describing the image while it takes a long time to render due to poor internet connection. Or...it would provide text for the image and could be used for visually impaired people that have to use text readers.

2. How can you improve accessibility of images in an HTML document?

By using figures, captions and alt text. Both captions and alt text would appear in events of images not working/loading.

3. Provide an example of when the figure element would be useful in an HTML document.

- Express meaning in a way thats easier to grasp
- Provides essential information that supports the main text
- To provide a semantic container and clearly link the figure to the caption

4. Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

A GIF image, granny, is usually an animated image that just loops itself and plays a short snippet but can also be just an image. SVG images are ideal for icons, diagrams and things that require more accuracy at various sizes.

5. What image type would you use to display a screenshot on your website and why?

Lossless WebP or PNG. WebP is preference because it offers better compression and has a wider support for high color depths. PNG is a nice fallback as it has reproduces sourced images better than JPEG but not as well as WebP. PNG browser support is better than WebP though so could be the better choice.

## CSS: Color and HTML Text elements
[Color](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color)
[HTMLTextElements](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

1. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

Foreground color just  applys to the HTMLs element content and will be displayed BEFORE the background color. You may set background to black but if you place a foreground color of blue it will show up over the black background.

2. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

First I would tell them to [read](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color#using_color_wisely) this and then ask them what emotion they want with their content. Maybe even have them peruse color palette websites like [this](https://colorhunt.co/) to find an example or pick one out from there.

3. What should you consider when choosing fonts for an HTML document?

Ensure that they are web safe fonts- widely used and available on multiple different OS.

4. What do font-size, font-weight, and font-style do to HTML text elements?

- font-size: takes values measured in multiple different units and makes the font different sizes 
- font-weight: sets how bold the text is
- font-style: used to turn italic on or off

5. Describe two ways you could add spacing around the characters displayed in an h1 element.
      1. Add spacing with a `<p>` element and then in our CSS we would add it to our h1 with `h1 + p {...` 

      2. Adding a `line-height` property 



## Things I want to learn more about
Best color schemes for businesses, personal usage and generally just more about colors for websites. 

Different ways to change/add rules in CSS by combining semantic elements

The voodoo of the lecture today in which the static and relative positions of 'fixed' and 'Absolute' were displayed when hovered over.