# php-slim-rest
Add custom response model
<br>
<hr>
<b>ResponseModel</b>
<br>
string $message;
<br>
bool $success;
<br>
function setMessage(string $message);
<br>
<hr>
<b>ResponseSuccessModel <i>extends</i> ResponseModel</b>
<br>
constructor => $success = true;
<br>
<hr>
<b>ResponseErrorModel <i>extends</i> ResponseModel</b>
<br>
constructor => $success = false;
<br>

<hr>
<b>ResponseDataModel <i>extends</i> ResponseModel</b>
<br>
$data;
<br>
function setData($data);
<br>
<hr>
<b>ResponseSuccessDataModel <i>extends</i> ResponseDataModel</b>
<br>
constructor => $success = true;
<br>
<hr>
<b>ResponseErrorDataModel <i>extends</i> ResponseDataModel</b>
<br>
constructor => $success = false;
<br>
<h2>Use</h2>
<br>
(new ResponseSuccessModel())<br>
&nbsp;&nbsp;->setMessage("Successful");
<br>
(new ResponseSuccessDataModel())<br>
&nbsp;&nbsp;->setMessage("Successful")<br>
&nbsp;&nbsp;->setData($posts);

