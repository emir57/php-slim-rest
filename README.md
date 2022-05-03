# php-slim-rest

Add custom response model
<br>
<hr>
ResponseModel
<br>
string $message;
<br>
bool $success;
<br>
function setMessage(string $message);
<br>
<hr>
```diff
ResponseSuccessModel  - extends ResponseModel
```
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorModel ```diff - extends ``` ResponseModel
<br>
constructor => $success = false;
<br>

<hr>
ResponseDataModel ```diff - extends ``` ResponseModel
<br>
$data;
<br>
function setData($data);
<br>
<hr>
ResponseSuccessDataModel ```diff - extends ``` ResponseDataModel
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorDataModel ```diff - extends ``` ResponseDataModel
<br>
constructor => $success = false;
<br>

