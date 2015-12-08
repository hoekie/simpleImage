# simpleImage

An image helper for Simple MVC Framework

Include this class in your controller

<pre><code>
use Helpers\SimpleImage;
</code></pre>

<pre><code>
$img = new SimpleImage('image.jpg');
$img->flip('x')->rotate(90)->best_fit(320, 200)->sepia()->save('result.gif');
</code></pre>
