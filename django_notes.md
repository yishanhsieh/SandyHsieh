<h1>Django learning notes</h1>




<h2>網路問題真的很痛苦</h2>
<p>2021/6/6~6/20<br>這兩周工作比較忙，平日能寫玩code的時間變少，且又遭遇兩個主要網路問題: <BR>

**1. VM SSH連線失敗: 我是用Bitvise，但ssh連線噴**

`Connection failed. FlowSocketConnector: Failed to connect to target address. Windows error 10061: No connection could be made because the target machine actively refused it.`

後來修改連線資訊，原本我是填連線到IPV4的網址(192.xxx.xxx.xxx), 後來改成 127.0.0.1(想想滿白癡的，VM網路連線我設定ss的主機IP是127.0.0.1，兩者不合當然不通。)

**2. Localhost 開不起 Django admin**

runserver有成功訊息，但127.0.0.1:8000就是failed to connect。<br>爬了文，我試著runserver其他PORT, allowed host改成[127.0.0.1:8000]，但都沒有成功。後來也是滿神奇的，裝上ngrok後，我重新runserver, allowed host改回預設["*"]，local突然可以連了:confused: 之後有空再重裝一次看看會不會重現問題好了，總覺得沒完全弄懂。


* reference:
    * [Alan Tsai學習筆記](https://blog.alantsai.net/posts/2018/04/devtooltips-5-ngrok-allow-public-to-access-localhost-website-and-sql-server)
    * [ngrok](https://ngrok.com/)
</p>


---
<h2>CSS + HTML basic</h2>
<p>2021/6/5~6/6<br>Ubuntu安裝教學，通常都會教裝apache, 讓你可以在local端build起 helloWorld。於是中間我花了點時間，先練習html, css。做了一個靜態網頁練習:<br>

* [Tribute page](https://codepen.io/yishanhsieh/pen/oNZdZoL)
</p>


---

<h2>Start from Installing Ubuntu</h2> 
<p>2021/5/29~30</br>以前公司線上會議時，常常看到工程師的螢幕分享是Ubuntu的畫面，因此我想，要學寫程式，就從安裝Ubuntu開始吧!當時也沒想太多，只想要灌雙系統，於是爬到一篇號稱是 "保母式教學"的文章，我照上面切磁碟空間、也找了usb裝Ubuntu，但是在最後一步，開BIOS重啟系統時，卻一直無法看到Ubuntu的安裝UI。<br>問了搞韌體的哥哥，但他給我的良心建議是改去用VM，因為這樣Ubuntu被我搞壞了，也不至於有根本性破壞。Youtube上有非常多VM教學，基本上全新手，不到半小時就架起來了，Ubuntu也灌好了。


* reference:
    * [Everyone needs to learn linux](https://www.youtube.com/watch?v=l9YxTXDiiFY&t=718s)
    * [(保姆式教學) Win10 + Ubuntu 20.04](https://www.gushiciku.cn/pl/gfr7/zh-tw)
    * [Host FREE website @ Home 1 - Build a Linux Server](https://www.youtube.com/watch?v=uyF3gC9lQtE&t=2s)
    * [Host FREE website @ Home 2 - Apache2 & Port Forwarding](https://www.youtube.com/watch?v=KvLj-TNXFDs&t=484s)

</p>