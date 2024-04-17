https://blog.csdn.net/m0_58416529/article/details/136098186  
找到Typora安裝目錄，依次找到這個檔案
```
resources\page-dist\static\js\LicenseIndex.**********.********.chunk.js 

用記事本打開它，

查  找【e.hasActivated="true"==e.hasActivated,】

取代為【e.hasActivated="true"=="true",】
```

在Typora安裝目錄依次找到這個檔案

resources\page-dist\license.html

用記事本打開它，
```
查  找【</body></html>】

取代為

</body><script>window.onload=function(){setTimeout(()=>{window.close();},5);}</script></html>
```
04、去除軟體左下角“未啟動”提示
在Typora安裝目錄依次找到這個檔案
```
resources\locales\zh-Hans.lproj\Panel.json 

查  找【"UNREGISTERED":"未啟動",】

取代為【"UNREGISTERED":" ",】
```
