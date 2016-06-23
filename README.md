## Simple Slim Framework File Response

using this package you can simply make http file response.
so what FileResponse class does is, set needed http headers for file response
and also getResponse method has an optional third parameter which you can provide when you want http client
save file as a name other than the name which stored on server.

## Sample usage

```php

$app->get('/test/image',function($request, $response){

    $filePath = '/path/to/your/image/file';

    return mhndev\slimFileResponse\FileResponse::getResponse($response, $filePath);
});



$app->get('/test/pdf',function($request, $response){

    $filePath = '/path/to/your/pdf/file';

    return mhndev\slimFileResponse\FileResponse::getResponse($response, $filePath ,'myDocument');
});



```
