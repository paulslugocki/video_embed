## Video embed

### Simple example

```php

include("video_embed.php");
$vid = new VideoEmbed();
echo $vid->get_embed("YE7VzlLtp-4");

```
Generates:

```html

<iframe width="420" height="315" src="http://www.youtube.com/embed/YE7VzlLtp-4?rel=0" frameborder="0" allowfullscreen></iframe>

```

### Specify the service

```php

include("video_embed.php");
$vid = new VideoEmbed();
echo $vid->get_embed("1084537", "vimeo");

```
Generates:

```html

<iframe src="http://player.vimeo.com/video/1084537" width="420" height="315" frameborder="0" allowFullScreen></iframe>

```

## Options





