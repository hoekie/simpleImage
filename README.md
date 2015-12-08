# simpleImage

An image helper for Simple MVC Framework.

Deal with images with this excelent piece of code from Cory LaViska from http://www.abeautifulsite.net!

Features:

flip() – flips an image vertically or horizontally<br />
rotate() – rotates an image at the specified angle<br />
auto_orient() – adjusts the orientation based on the image’s EXIF data<br />
resize() – resizes an image to the specified width/height<br />
fit_to_width() – proportionally resizes an image to the specified width<br />
fit_to_height() – proportionally resizes an image to the specified height<br />
best_fit() – proportionally resizes an image to fit within the specified width/height<br />
crop() – crop an image from x1/y1 to x2/y2<br />
square_crop() – trim the image to a square and resize to the specified size<br />
desaturate() – convert the image to grayscale<br />
invert() – invert the image<br />
brightness() – adjust the image’s brightness<br />
contrast() – adjust the image’s contrast<br />
colorize() – apply the colorize filter<br />
edges() – apply the edges filter<br />
emboss() – apply the emboss filter<br />
mean_remove() – apply the mean removal filter<br />
blur() – apply selective or gaussian blur to the image<br />
sketch() – apply the sketch filter<br />
smooth() – apply the smooth filter<br />
pixelate() – pixelate the image to blocks of the specified size<br />
sepia() – apply a simulated sepia effect<br />
overlay() – overlay one image onto another to create a watermark effect<br />
text() – Add text to the image<br />

#### How to use:

Copy the helper to the app\helpers dirctory and include this class in your controller:

<code>
use Helpers\SimpleImage;
</code>

Then create a new instance of the image helper:

<code>
$img = new SimpleImage('image.jpg');
</code>

#### Example:

This will load image.jpg, flip it horizontally, rotate it 90 degrees, shrink it to fit within a 320×200 box, apply a sepia effect, convert it to a GIF, and save it to result.gif:

<code>
$img->flip('x')->rotate(90)->best_fit(320, 200)->sepia()->save('result.gif');
</code>

For more examples, visit [http://www.abeautifulsite.net/the-simple-image-class-for-php](http://www.abeautifulsite.net/the-simple-image-class-for-php).

#### Credits:

All credits goes to LaViska at [http://www.abeautifulsite.net](http://www.abeautifulsite.net).
