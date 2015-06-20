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
- 1.網頁語言設定成「utf-8」
- 2.在head裡，打上標題<title>熊貓家族</title>，這樣網頁最上面的瀏覽標籤就會跑出熊貓家族
- 3.設定連結(link)，‵`<link rel="stylesheet" type="text/css" href="css/bootstrap.css">‵`
``
    <div class="container">
      <div class="row well well-lg">
``
