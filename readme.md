# Boofw\Flysystem\Qiniu

This is a Flysystem adapter for the Qiniu.

```bash
composer require boofw/flysystem-qiniu
```

# Bootstrap

``` php
<?php
use League\Flysystem\Filesystem;
use Boofw\Flysystem\Qiniu\QiniuAdapter as Adapter;

$ak = '**********';
$sk = '**********';
$bucket = 'bucket-name';

$filesystem = new Filesystem(new Adapter($ak, $sk, $bucket));
```
