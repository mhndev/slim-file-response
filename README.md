## Simple Slim Framework File Response

## Sample usage

```php

$app->get('/test/image',function($request, $response){

    $filePath = '/path/to/your/image/file';

    return mhndev\slimFileResponse\FileResponse::getResponse($response, $filePath);
});



$app->get('/test/pdf',function($request, $response){

    $filePath = '/path/to/your/pdf/file';

    return mhndev\slimFileResponse\FileResponse::getResponse($response, $filePath);
});



```
