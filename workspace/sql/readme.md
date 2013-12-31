修改 `manifest.xxx/config.php` 檔案，添加下列 Dump DB 設定：

若添加 `'dump' => 'download'` 則不會儲存於主機，會立即驅動下載。

若使用 `'dump' => 'text'` 則會於瀏覽器直接顯示，自行複製使用。

###### DUMP_DB ######
'dump_db' => array(
    'format' => '%1$s-'.date('Ymd').'.sql',
    'path' => '/workspace/sql',
    'restore' => 'yes'
),
########

ps. 若要製作 Ensemble，就不能刪除掉 `install` 目錄。