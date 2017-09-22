# wordpress
<h1>Отправить файл через ajax запрос для wordpress</h1>
var file_data = jQuery('#rewrite-maket').prop('files')[0];<br />
var form_data = new FormData();<br />
form_data.append('file', file_data);<br />
form_data.append('action', 'rewrite_makets_action');
<br />
jQuery.ajax({<br />
  url: myajax.url,<br />
  type: 'post',<br />
  contentType: false,<br />
  processData: false,<br />
  data: form_data,<br />
  success: function (response) {<br />
  }<br />
});<br />
