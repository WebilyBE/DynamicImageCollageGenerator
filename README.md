### Dynamic Image Collage Generator
This PHP script dynamically generates images based on various parameters such as image width and height, text to be displayed, and the presence of image files. Here is a detailed description of the code:

1. **Folder and File Checks:**
- The code starts by defining the paths to the folders where images are stored and retrieved from.
- If the folders do not exist, they are created with the appropriate permissions.

2. **Image Count Check:**
- If there are fewer than 4 images in the specified folder, a default image is generated with a background color and text.

3. **Color Interpolation:**
- Two functions are defined to interpolate colors between different images, namely `interpolateColor()` and `getLighterColor()`.
- These functions calculate colors based on the available images to create a smooth transition of colors.

4. **Generate Background Image:**
- If there are enough images, a new image is created with the specified width and height.
- The code divides the image space into four equal parts and applies a color gradient between the colors of the four images.

5. **Add Text:**
- The code optionally adds text to the generated image.
- The text is centered on the image and a rectangular background around the text is drawn.

6. **Combine Images:**
- The code places the images in a grid on the background image.
- The images are scaled and centered at their respective locations based on the size of the background image.

7. **Save and Output Image:**
- The generated image is saved with a unique filename in the specified folder.
- The image is then directly output as a JPEG image.

This script generates dynamic image collages with text overlay, which is useful for automatically creating attractive visuals for social media posts, for example.

Here are some example links to generate dynamic image collages:

1. **Dynamic Collage**: This link generates a dynamic image collage with a width of 1200 pixels, a height of 630 pixels, and the text "Dynamic Collage". `example.com/generate_image_collage.php?width=1200&height=630&text=Dynamic%20Collage`

2. **Awesome Collage**: This link creates an awesome image collage with a width of 638 pixels, a height of 404 pixels, and the text "Awesome Collage".  `example.com/generate_image_collage.php?width=638&height=404&text=Awesome%20Collage`

3. **Beautiful Collage**: Use this link to generate a beautiful image collage with a width of 600 pixels, a height of 315 pixels, and the text "Beautiful Collage". `example.com/generate_image_collage.php?width=600&height=315&text=Beautiful%20Collage`

You can replace `example.com/generate_image_collage.php` with the actual URL where the script is hosted.
