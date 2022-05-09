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
            public function __construct()
            {
                $this->success = true;
            }
}
```
<hr>

```php
class ResponseErrorModel extends ResponseModel{
            public function __construct()
            {
                $this->success = false;
            }
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
            public function __construct()
            {
                $this->success = true;
            }
}
```

<hr>

```php
class ResponseErrorDataModel extends ResponseDataModel{
            public function __construct()
            {
                $this->success = false;
            }
}
```

<h2>Use</h2>

```php
(new ResponseSuccessModel())
            ->setMessage("Successful");
```

```php
(new ResponseSuccessDataModel())
            ->setMessage("Successful")
            ->setData($posts);
```
            


