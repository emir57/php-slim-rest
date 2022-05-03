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
ResponseSuccessModel extends ResponseModel
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorModel extends ResponseModel
<br>
constructor => $success = false;
<br>

<hr>
ResponseDataModel extends ResponseModel
<br>
$data;
<br>
function setData($data);
<br>
<hr>
ResponseSuccessDataModel extends ResponseDataModel
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorDataModel extends ResponseDataModel
<br>
constructor => $success = false;
<br>

