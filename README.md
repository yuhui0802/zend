# ubuntu zend 3 install 
下載composer.phar

curl -sS https://getcomposer.org/installer | php

進去想要把專案放在哪個資料夾(未來就是此路徑提供網頁服務)運行安裝

php composer.phar create-project -sdev zendframework/skeleton-application myzend

基本上跑完就能運行了，但自己有遇到一個問題，問題訊息如下：

Invalid command 'RewriteEngine', perhaps misspelled or defined by a module not included in the server configuration

上網查詢解決方式：
指令：a2enmod rewrite
指令：systemctl restart apache2   #重啟apache2
