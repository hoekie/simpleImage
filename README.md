# simpleImage

An image helper for Simple MVC Framework.

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
