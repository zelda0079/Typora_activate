# 方法1
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
==========================================================

# 方法2
~~https://github.com/743859910/Typora_Unlocker~~  
https://github.com/L1ne-cd/Typora_Unlocker  
https://gitcode.com/gh_mirrors/ty/Typora_Unlocker/  

1. 下載補丁  
下載2個檔案，解壓。


2. 移入目錄
將這license-gen.exe和node_inject.exe這2個檔案放到 typora的運行目錄，就是安裝目錄


3. 執行命令
打開cmd命令列，進入到Typora的安裝目錄，執行2個命令列
```
# 自動組態相關檔案`
.\node_inject.exe
# 序列號生成
.\license-gen.exe
```
如圖所示，他就會給你一個序列號，然後你輸入進去就行


4. 輸入序列號
將上面的序列號輸入進去，信箱的話隨便填寫都可以

