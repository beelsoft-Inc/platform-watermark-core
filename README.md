# Watermark for laravel-admin

Add Text Watermark in Laravel-admin web page.


## ScreenShot

<img src="https://user-images.githubusercontent.com/2421068/85280542-e65d1c80-b4ba-11ea-842f-09c2a0e1dc5e.png">

## Install

```bash
composer require jxlwqq/watermark
```

## Configurations

Add `extensions` option in your `config/admin.php` configuration file:

```php
'extensions' => [
    'watermark' => [
        'enable' => true,
        'config' => [
            'content' => 'username', // Admin::user()->username, or Admin::user()->name or fixed value like 'internal info'
            'width' => '100px',
            'height' => '120px',
            'textAlign' => 'left',
            'textBaseline' => 'alphabetic',
            'font' => '15px Times New Roman',
            'fillStyle' => 'rgba(204,204,204,0.4)',
            'rotate' => 30,
            'zIndex' => 1000,
        ]
    ]
]
```

## License

Licensed under [The MIT License (MIT)](LICENSE).
