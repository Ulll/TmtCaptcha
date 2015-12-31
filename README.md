# heil.captcha

##description

This library based on [cool-captcha](https://code.google.com/p/cool-php-captcha/)

enjoy it!!!

##usage

```php
  
require_once './Captcha.php';

$config = array(
  'img_path' => $this->_img_path,
  'img_url' => $this->_img_url,
  'minWordLength' => $this->_minWordLength,
  'maxWordLength' => $this->_maxWordLength,
  'fonts' => array(
      'VeraSansBold' => array('spacing' => 0, 'minSize' => 18, 'maxSize' => 18, 'font' => 'VeraSansBold.ttf')
  ),
  'width' => $this->_width,
  'height' => $this->_height,
  'expiration' => $this->_expiration,
);
$cap = new TMTCaptcha($config);
$captcha = $cap->createImage();

```

##example

![example1](https://github.com/Ulll/heil.captcha/blob/master/example/1451531306.8061.jpg)
![example2](https://github.com/Ulll/heil.captcha/blob/master/example/1451531331.0574.jpg)
![example3](https://github.com/Ulll/heil.captcha/blob/master/example/1451531339.0852.jpg)
![example4](https://github.com/Ulll/heil.captcha/blob/master/example/1451531353.1939.jpg)
