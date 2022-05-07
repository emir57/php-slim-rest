# php-slim-rest
Add custom response model
<br>


```php
class ResponseModel{
            string $message;
            bool $success;
            function setMessage(string $message);
}
```
<hr>

```php
class ResponseSuccessModel extends ResponseModel{
            constructor => $success = true;
}
```
<hr>

```php
class ResponseErrorModel extends ResponseModel{
            constructor => $success = false;
}
```
<hr>

```php
class ResponseDataModel extends ResponseModel{
            $data;
            function setData($data);
}
```
<hr>

```php
class ResponseSuccessDataModel extends ResponseDataModel{
            constructor => $success = true;
}
```

<hr>

```php
class ResponseErrorDataModel extends ResponseDataModel{
            constructor => $success = false;
}
```

<h2>Use</h2>

```php
(new ResponseSuccessModel())
            ->setMessage("Successful");

(new ResponseSuccessDataModel())
            ->setMessage("Successful")<br>
            ->setData($posts);
            
```

