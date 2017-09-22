# wordpress
<h1>Отправить файл через ajax запрос для wordpress</h1>
var file_data = jQuery('#rewrite-maket').prop('files')[0];
var form_data = new FormData();
form_data.append('file', file_data);
form_data.append('action', 'rewrite_makets_action');
//Имя файла которое хотим заменить
form_data.append('file-name', $('#tab-pages .tab-content-pages .tab-pane-page.active').data('parse-file'));

jQuery.ajax({
  url: myajax.url,
  type: 'post',
  contentType: false,
  processData: false,
  data: form_data,
  success: function (response) {
  }
});
