<html>
<head>
<title>Page Title</title>
<script>
    function startTime(){
      var today = new Date();
      var hh = today.getHours();
      var mm = today.getMinutes();
      var ss = today.getSeconds();
      mm = checkTime(mm);
      ss = checkTime(ss);
      document.getElementById('clock').innerHTML = today + hh + ":" + mm + ":" + ss;
      var timeoutId = setTimeout(startTime, 500);
    }
    function checkTime(i){
      if(i < 10) {
        i = "0" + i;
      }
      return i;
    }  
</script>
<style>
body {
  background-color: black;
  text-align: left;
  color: #B3EE3A;
  font-family: Arial, Helvetica, sans-serif;
}
t {
 color:yellow;
}
h1 {
  color:#D94DFF;
}
</style>
<style>
 <!--
	A:link {color: yellow; font-family: 標楷體}
	A:visited {color: gray; font-family: 標楷體}
	A:active {text-decoration: none; font-family: 標楷體}
	A:hover {text-decoration: none; color: red}
 -->
</style>
</head>
  
<body onload="startTime()">

<t><font face="標楷體" size="7">許乃懿</font></t>

<h1><b><font face="Arial" size="6">ABOUT ME</font></b></h1>
<img src="ME.jpg" style="width:200px">
<p>清華大學  資訊工程學系</p>
<p>斗六高中</p>
<p>斗六國中</p>

<hr size="5" align="center" noshade width="90%" color="0000ff">

<h1><b><font face="Arial" size="6">INTERESTS</font></b></h1>
<p>壘球 籃球</p>
<p>刺客教條 英雄聯盟</p>
<p>看書 睡覺</p>

<hr size="5" align="center" noshade width="90%" color="0000ff">

<h1><b><font face="Arial" size="6">BOOKS</font></b></h1>
<p>1.福爾摩斯</p>
<p>2.1984</p>
<p>3.分歧者</p>

<hr size="5" align="center" noshade width="90%" color="0000ff">

<h1><b><font face="Arial" size="6">CONNECTIONS</font></b></h1>
<p>email：<a href="vmsu11051105@gmail.com">vmsu11051105@gmail.com</a></p>
<p>facebook：<a href="https://www.facebook.com/profile.php?id=100008588917658">許乃懿</a></p>

<hr size="5" align="center" noshade width="90%" color="0000ff">

<h1><b><font face="Arial" color="#00FFFF" size="6"><marquee behavior="scroll">Nothing is true<br>Everything is permitted</marquee></font></b></h1>

<p>現在時間</p>
<div id="clock"></div>

</body>
</html>
