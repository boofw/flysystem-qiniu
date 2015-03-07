# Polev\Flysystem\Qiniu

This is a Flysystem adapter for the Qiniu.

```bash
composer require polev/flysystem-qiniu
```

# Bootstrap

``` php
<?php
use League\Flysystem\Filesystem;
use Polev\Flysystem\Qiniu\QiniuAdapter as Adapter;

$ak = '**********';
$sk = '**********';
$bucket = 'bucket-name';

$filesystem = new Filesystem(new Adapter($ak, $sk, $bucket));
```
