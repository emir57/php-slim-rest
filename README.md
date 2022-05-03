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
ResponseSuccessModel <span style="color:#884EA0;">extends</span> ResponseModel
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorModel <span style="color:#884EA0;">extends</span> ResponseModel
<br>
constructor => $success = false;
<br>

<hr>
ResponseDataModel <span style="color:#884EA0;">extends</span> ResponseModel
<br>
$data;
<br>
function setData($data);
<br>
<hr>
ResponseSuccessDataModel <span style="color:#884EA0;">extends</span> ResponseDataModel
<br>
constructor => $success = true;
<br>
<hr>
ResponseErrorDataModel <span style="color:#884EA0;">extends</span> ResponseDataModel
<br>
constructor => $success = false;
<br>

