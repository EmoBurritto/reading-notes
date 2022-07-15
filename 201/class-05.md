# Images, Color, Text

## Using Images In HTML

img element used to add simple images on a page; empty element, uses src attribute like href is used for a element in a relative URL. figure element is used to add captions to an image or multimedia source. For img element you can assign a file path or file name besides the URL for the src attribute. Don't do "hotlinking", referncing someone else's page without their permission to display their image; copy rights are a huge deal. img and video element are sometimes referred as replaced elements; size defined by external source. Easiest way to test alt message, mispell file name or URL to see user's interaction to page. For decoration use alt element; helps screen reader identify what is and isn't important. If image contains a lot of info, use alt element to copy info for user. Image in an a element turns into URL. width and height affect size of image. use title attribute to add supportign information about txt. figire and figcaption element to use captions for image. background- image helps place a URL in the background of site.

(references: <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML>)

## Common Image Types, Choosing Image Formats

APNG is for lossless GIF's. AVIF is for good for both both high quality images and animated images. GIF is for simple image and animations. JPEG is good for lossy compression of still images. APNG was built upon by PNG. BMIP good for windows user but avoid to represent data. 

(references: <https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types>)

## Questions

1. What is a real world use case for the alt attribute being used in a website?

Slow internet to display image, description there for user.

2. How can you improve accessibility of images in an HTML document?

By using alt. it helps screen reader for impaired users to get full user experience as the coder intended.

3. Provide an example of when the figure element would be useful in an HTML document.

If an impaired user is on a site and can't really take in the images or site he sees in full detail, figure element can help with hashing out the details.

4. Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

gif- compressed 8-bit image; simple animation
svg- test files that include code that draw images; diagrams 

5. What image type would you use to display a screenshot on your website and why?

JPEG since its the most used for still images; lossless format

## Using Color in CSS

Using Color is so infintie due to the RGB wheel. There was a lot of attributes and properties that can affect the color of literally anything in the page. This will help style up the CSS portion of the page although have to keep in mind color theory and user friendliness, don't want too much going on at once. 

(references: <https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color>)

## Styling HTML Text Elements

Styling HTML text elements can be super specific or apply toi a general area. These page had a lot of properties and it helps with what we learned so we can style the page as we like down to a T. I feel like it's abit overwheelming and feel there's a right and wrong answer when it comes to clean CSS code. Is there a way to check that one attribute over rides another? Like attribute flow order like how the computer analyzes the code files. 


(references: <https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals>)

## Questions

1. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

- foreground: affect color of space around txt

- background colors: affect the type of color used on whole website 

2. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

- background-color, color; connsider color theory and and color blindness for user friendliness

3. What should you consider when choosing fonts for an HTML document?

- web sapce fonts; font-family; color

4. What do font-size, font-weight, and font-style do to HTML text elements?

- font-size: affects the size of the txt in given HTML element in ist setting

- font-weight: boldness of the txt

- font-style: affect the type of font used

5. Describe two ways you could add spacing around the characters displayed in an h1 element.

- By using letter-spacing and word-spacing it affects the relatioship of the letters and word next to them, they can take most height and width size units. 

## Things I want to know more
- image types in the real world 
- do people really memorize the stuff
- how much CSS is too much CSS
- what is clean CSS