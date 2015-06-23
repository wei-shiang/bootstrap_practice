#  Wei-Xiang's notes
## 一、先安裝Git Bash 與 Sublime Text
### 二、A.下載Bootstrap的檔案
- 到Bootstrap的網站，點Download
- 選第一個"Download Bootstrap"後，會下載Zip檔
- 解壓縮檔案，並把「css、fonts、js」三個資料夾，複製到我們網頁的資料夾「bootstap_practice」
- 把「Bootstap_practice」資料夾丟進Sublime Text
- 新增file，命名為index.html，打html按Tab鍵，就能跑出架構

### B.到老師的Git hub下載檔案
- 辦好Git hub帳號後，搜尋老師(andystu) 找檔案「bootstrap_practice」按進去後，點Fork
- 到自己的頁面，點「bootstrap_practice」，就去後右下角複製連結
- 到Git Bash 打git clone 貼上剛才複製的連結
- 載好後，到C曹Site資料夾裡就能看見「bootstrap_practice」資料夾，並把他丟進Sublime Text

###三、選定主題後就開始吧~
- 網頁語言設定成「utf-8」
- 在head裡，打上標題<title>熊貓家族</title>，這樣網頁最上面的瀏覽標籤就會跑出熊貓家族
- 設定link，打``<link rel="stylesheet" type="text/css" href="css/bootstrap.css">`` 不然無法與bootstrap.css連結
- 設定link，打``<link rel="stylesheet" type="text/css" href="css/bootstrap.css">`` 不然不能與 main.css連結

###四、排版
- ``<div class="container">``
- ``<div class="row well">`` => row是這段變成一個區塊，well是這段會有個框
- ``<div class="col-md-6">`` => 每行最多12，若要分欄相加不可以超過12，不然第二欄會換到下一行。
- ``<h3>這裡放文章內容</h3>``
- ``</div>``
- ``<br/>`` =>可以換行
- ``<div class="col-md-6>``
- ``<img src="這裡放照片的連結網址" style="width:90%">`` width可以設定照片的大小。
- ``</div>``
- ``</div>``
- ``</div>`` =>這段調col-md-6，所以會分兩欄

###五、頁腳
-  ``<footer class="container-fluid">``  =>滿版
-  `` <div class="row">``
-  `` <div class="container">``
-  `` <div class ='col-md-3'>``
-  ``<h1><font size="5">好站連結</font></h1>``  =>頁腳的標題
-  ``<ul class="list-unstyled">``  =>把連結的點點去掉
-  `` <li><a href="放網址" target= _blank">台北市大貓熊保育網</a></li>`` =>_blank是開新頁
-  ``<li><a href="http://www.zoo.gov.taipei/" target="_blanK">台北市立木柵動物園</a></li>``
-  ``</ul>``
-  ``</div>``
-  ``</div>``
-  ``</div>``
-  ``</footer>``
- 開 main.css ‵`footer{background-color :#FFF;}`` =>調頁腳的背景顏色

###六、glyphicon
- ``<div class="container feature">`` =>要在上一層的div 加上 feature ((不然會有問題
- ``<i class="glyphicon glyphicon-home">`` =>到Bootstrap -> Components 選擇要的icon 複製
- 貼到  "    " 裡面
- 到main.css 打上``.feature .glyphicon {font-size :26px;}`` ((可設定icon的大小

###七、設定頁首
- ``<div class="navbar navbar-default navbar-fixed-top">`` =>navbar-default 設定導覽列的樣式 (白色的)、fixed-top固定在上列
- ``<div class="container">``
- ``<a href="index.html" class="navbar-brand">熊貓家族</a>`` => 標題會浮動靠左對齊
- ``<ul class="nav navbar-nav navbar-right ">`` =>導覽列靠右對齊
- ``<li><a href="index.html"><i class="glyphicon glyphicon glyphicon-home " title="回首頁"></i></a></li>`` 
-   =>把glyphicon結合導覽列，並超連結至首頁。
- ``<li><a href="2.html"><i class="glyphicon glyphicon-film" title="可愛影片"></i></a></li>`` =>超連結到2.html(可愛影片)
- ``<li><a href="1.html"><i class="glyphicon glyphicon-file" title="分辨訣竅"></i></a></li>`` =>連結到1.html (分辨秘訣)
- ``</ul>``
- ``</div>``
- ``</div>``
- 因為是用固定在最上列，下面的文字會跑版，因此要到main.css設定間距
- ``body{padding-top : 100px;}`` 
 
###八、設定手機大小瀏覽，導覽列會藏起來
- 把原本的頁首部分，變成這樣
- ``div class="navbar navbar-default navbar-fixed-top">`` 
- ``<div class="container feature">``
- ``<div class="navbar-header">`` =>可讓下拉式清單展開後滿版排好
- ``<a href="index.html" class="navbar-brand"><font size="5">熊貓家族</font></a>``
- ``<button type="button" class="navbar-toggle" data-toggle="collapse"   data-target=".navbar-collapse">``=>設定會在小型視窗隱藏
- ``<span class="sr-only">Toggle navigation</span>``
- ``<span class="icon-bar"></span>`` =>icon 增加一條線
- ``<span class="icon-bar"></span>``
- ``<span class="icon-bar"></span>``=>想多一點線可以多打幾個
- ``</button>``
- ``</div>``
- ``<ul class="nav navbar-nav navbar-right nave collapse navbar-collapse">`` 
- =>collapse 加在有nav的後面，navbar-collapse 除了手機以外的都會顯示出來
- ``<li><a href="index.html"><i class="glyphicon glyphicon glyphicon-home " title="回首頁"></i></a></li>``
- ``<li><a href="2.html"><i class="glyphicon glyphicon-film" title="可愛影片"></i></a></li>``
- ``<li><a href="1.html"><i class="glyphicon glyphicon-file" title="分辨訣竅"></i></a></li>``
- ``</ul>``
- ``</div>``
- ``</div>``
 
###八、改字、頁面的顏色
- 在main.css 更改
- ``body{background-color :#000;}`` 更改背景顏色  ((#000為黑色
- ``h2{color :#FFF;}`` <h2>的顏色通通是白色
- 若要單獨改字顏色與大小直接在字那邊改，不用到main.css``<h4><font size="6" color="blue">圓仔</font></h4>`` 
