**1)** add repositories to package.json file

``` php
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/Mehdikarimian/ExcelBundle"
        }
    ]
``` 
(example) 
``` php
{
    "type": "project",
    "license": "proprietary",
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/Mehdikarimian/ExcelBundle"
        }
    ],
    "require": {
        "php": "^7.1.3",
        "ext-iconv": "*",
        "Mehdikarimian/excelbundle": "dev-master",
        "beberlei/DoctrineExtensions": "^1.0",
        "friendsofsymfony/user-bundle": "^2.1",
        "sensio/framework-extra-bundle": "^5.1"
    },
    "require-dev": {
        "symfony/browser-kit": "^4.0",
        "symfony/css-selector": "^4.0",
        "symfony/debug-pack": "*",
        "symfony/dotenv": "^4.0",
        "symfony/phpunit-bridge": "^4.0",
        "symfony/profiler-pack": "*",
        "symfony/web-server-bundle": "^4.0"
    },
    
}
```
**2)** 
``` shell
    composer require Mehdikarimian/ExcelBundle:dev-master
```
**3)** Register the bundle in ``config\bundles.php``
``` php
    $bundles = [
        // ...
    Liuggio\ExcelBundle\LiuggioExcelBundle::class => ['all' => true],
    ];
```

