# heil.captcha

##description

This library based on [cool-captcha](https://code.google.com/p/cool-php-captcha/)

##usage

```php
  
require_once './TMTCaptcha.php';

$config = array(
  'img_path' => '/Users/xy/workspace/blog/captcha/images/',
  'img_url' => 'http://.....captcha/images/',
  'minWordLength' => 4,
  'maxWordLength' => 5,
  'fonts' => array(
      'VeraSansBold' => array('spacing' => 0, 'minSize' => 18, 'maxSize' => 18, 'font' => 'VeraSansBold.ttf')
  ),
  'width' => 120,
  'height' => 60,
  'expiration' => 60,
);
$cap = new TMTCaptcha($config);
$captcha = $cap->createImage();

```

##support config

* `img_path` - the captcha images stored location
* `img_url` - the captcha images url prefix
* `minWordLength` - the min word number show in the images
* `maxWordLength` - the max word number show in the images
* `fonts` - you can set a lot of font in the object
* `width` - the image width
* `height` - the image height
* `expiration` - the image liftime , when expired , the old images will deleted automatically
* `lines` - the disturb lines number on the image
* `spots` - the disturb pixel number on the image
* `backgroundColor` - the backgroundColor of the image eg:array(255, 255, 255)
* `colors` - the font color eg : array(array(27,  78,  181), array(22,  163, 35),array(214, 36,  7))
* `lineWidth` - Horizontal line number through the text, default : 0



##example

![example1](https://github.com/Ulll/heil.captcha/blob/master/example/1451531306.8061.jpg)
![example2](https://github.com/Ulll/heil.captcha/blob/master/example/1451531331.0574.jpg)
![example3](https://github.com/Ulll/heil.captcha/blob/master/example/1451531339.0852.jpg)
![example4](https://github.com/Ulll/heil.captcha/blob/master/example/1451531353.1939.jpg)
