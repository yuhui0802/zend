# ubuntu zend 3 install 
下載composer.phar

curl -sS https://getcomposer.org/installer | php

進去想要把專案放在哪個資料夾(未來就是此路徑提供網頁服務)運行安裝

php composer.phar create-project -sdev zendframework/skeleton-application myzend
