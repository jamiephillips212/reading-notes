# Images, Color, Text, and Work with Functions

## What is a real world use case for the alt attribute being used in a website?

A real world example of what to use an alt attribute would be to use it on an `<img>` element.  This helps with *several* things.

- Accessibilty (Screen Readers)
- Description in case the image does not load correctly.
- Information that has SEO value (What's in the image?)

## How can you improve accessibility of images in an HTML document?

Use an `alt attribute!`

## Provide an example of when the figure element would be useful in an HTML document

Figure elements provide semantic value to images. It relates a caption to an image directly. An example of this would be an image of someone and a caption of who they are:

<figure>

<img src="mochi-is-awesome.jpg" 
alt="a picture of mochi though her phone camera broke and she needs to get it fixed." />

<figcaption>A sighting of mochi out of her cave.</figcaption>

</figure>
By containing the above in a clear container it improves SEO, accessability, and provides value beyond just a <p> tag.

## Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community

You would use a gif for a simple photo or an animation of several simple photos, like flipping an pages through a flipbook. You would use an svg image for when you need precise sizing such as for usable items on a webpage like a button.

## What image type would you use to display a screenshot on your website and why?

I would use a PNG because it is lossless and that's what MDN told me to do.

## Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge

You can generally think of the foreground being the color of a font and the background being the color behind the font. Like writing on a notepad you can use a blue pen or any other color - that's your foreground. You can then either use yellow legal pad or white or any other color and that is your background.

## Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

I would create a color pallete for his website to give it a uniformed look that flows well together. I would create CSS rules to enforce the pallete and then refine the colors until his blog popped. Nam'sayin Scotty P?

## What should you consider when choosing fonts for an HTML document?

The most important thing to me is to make sure I am using a web safe font. I want my web site to look consistent on any platform or browser. This can be overcame by using font-stacks but again, I want a consistent experience. You should then also consider the readability and accessability of your chosen font; from size to color.

## What do font-size, font-weight, and font-style do to HTML text elements?

- font-style - This controls the italic aspects of a font.
- font-weight - This controls the boldness of a font.
- font-size - This controls the sizing aspect of the font.

## Describe two ways you could add spacing around the characters displayed in an h1 element

You can use letter-spacing or word-spacing.
