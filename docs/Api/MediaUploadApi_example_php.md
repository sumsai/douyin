###MediaUploadApi_mediaUploadPost
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Douyin\Open\Api\MediaUploadApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$open_id = "ba253642-0590-40bc-9bdf-9a1334b94059"; // string | 通过/oauth/access_token/获取，用户唯一标志
$access_token = "act.1d1021d2aee3d41fee2d2add43456badMFZnrhFhfWotu3Ecuiuka27L56lr"; // string | 调用/oauth/access_token/生成的token，此token需要用户授权。
$media = "media_example"; // string | 

try {
    $result = $apiInstance->mediaUploadPost($open_id, $access_token, $media);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MediaUploadApi->mediaUploadPost: ', $e->getMessage(), PHP_EOL;
}
?>
```
