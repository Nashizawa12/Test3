<!DOCTYPE html>
<html lang="en">
<head>
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="navbar">
            <img src="d:\music\Sound webpage_img\CHILLSPOT.png" class="logo">
            <ul>
                <li><a href="#">HOME</a></li>
                <li><a href="#">ABOUT</a></li>
                <li><a href="#">SPECIFICATIONS</a></li>
                <li><a href="#">PRODUCTS</a></li>
                <li><a href="#">CONNECT</a></li>
            </ul>
        </div>
        <div class="content">
            <div class="left-col">
                <h1>CHILL<br>SPOT</h1>
            </div>
            <div class="right-col">
                <p>Play</p>
                <img src="file:///d%3A/music/Sound%20webpage_img//play.png" id="icon">
            </div>
        </div>
    </div>
    <audio id="mySong">
        <source src="file:///d:/music/Sound%20webpage_img/Gustixa%20-%20Full%20Album%20_%20Tanpa%20iklan.mp3" type="audio/mp3">
    </audio>    
<script>
    var mySong = document.getElementById("mySong");
    var icon = document.getElementById("icon");
    icon.onclick = function(){
        if(mySong.paused){
            mySong.play();
            icon.src = "file:///d%3A/music/Sound%20webpage_img//pause.png";
        }else{
            mySong.pause();
            icon.src = "file:///d%3A/music/Sound%20webpage_img//play.png";
        }
    }
</script>
</body>
</html>
