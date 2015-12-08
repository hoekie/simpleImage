# simpleImage

An image helper for Simple MVC Framework.

Deal with images with this excelent piece of code from Cory LaViska from http://www.abeautifulsite.net!

Features:

flip() – flips an image vertically or horizontally
rotate() – rotates an image at the specified angle
auto_orient() – adjusts the orientation based on the image’s EXIF data
resize() – resizes an image to the specified width/height
fit_to_width() – proportionally resizes an image to the specified width
fit_to_height() – proportionally resizes an image to the specified height
best_fit() – proportionally resizes an image to fit within the specified width/height
crop() – crop an image from x1/y1 to x2/y2
square_crop() – trim the image to a square and resize to the specified size
desaturate() – convert the image to grayscale
invert() – invert the image
brightness() – adjust the image’s brightness
contrast() – adjust the image’s contrast
colorize() – apply the colorize filter
edges() – apply the edges filter
emboss() – apply the emboss filter
mean_remove() – apply the mean removal filter
blur() – apply selective or gaussian blur to the image
sketch() – apply the sketch filter
smooth() – apply the smooth filter
pixelate() – pixelate the image to blocks of the specified size
sepia() – apply a simulated sepia effect
overlay() – overlay one image onto another to create a watermark effect
text() – Add text to the image

#### How to use:

Copy the helper to the app\helpers dirctory and include this class in your controller:

<code>
use Helpers\SimpleImage;
</code>

Then create a new instance of the image helper:

<code>
$img = new SimpleImage('image.jpg');
</code>

<code>
$img->flip('x')->rotate(90)->best_fit(320, 200)->sepia()->save('result.gif');
</code>
