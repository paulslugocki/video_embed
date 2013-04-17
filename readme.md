# Video embed

Take a Youtube or Vimeo video ID and return the html embed code.

## Simple example

```php
include("video_embed.php");
$vid = new VideoEmbed();
echo $vid->get_embed("YE7VzlLtp-4");
```
Generates:

```html
<iframe width="420" height="315" src="http://www.youtube.com/embed/YE7VzlLtp-4?rel=0" frameborder="0" allowfullscreen></iframe>
```

### Options!

```php
include("video_embed.php");
$vid = new VideoEmbed();

$video_service = "vimeo"; // Defaults to "youtube"

$options = [
			"width" => 504,
			"height" => 378,
			"secure" => true
		];

echo $vid->get_embed("1084537", $video_service, $options);
```
Generates:

```html
<iframe src="http://player.vimeo.com/video/1084537" width="504" height="378" frameborder="0" allowFullScreen></iframe>
```



