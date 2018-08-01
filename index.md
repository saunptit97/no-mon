<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <meta http-equiv="Page-Enter" content="progid:DXImageTransform.Microsoft.Fade(duration=1)">
    <meta http-equiv="Page-Exit" content="progid:DXImageTransform.Microsoft.Fade(duration=1)">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <meta http-equiv="Content-Type" content="text/html; charset = UTF-8" />
    <link rel="shortcut icon" href="favicon.ico" />
    <link rel="Stylesheet" href="style.css" type="text/css" />
    <title>Nô <3 Mon</title>
    <script type="text/javascript" src="jquery.min.js"></script>
    <script type="text/javascript" src="counterup.js"></script>
    <script type="text/javascript" src="timroi.js"></script>
    <script language="javascript">

        title_tmp1 = document.title

        if (title_tmp1.indexOf(">>") != -1) {

            title_tmp2 = title_tmp1.split(">>");

            title_last = "*~*" + title_tmp2[1];

            title_last = title_last + "*~*" + title_tmp2[2];

        } else {



            if (title_tmp1.indexOf("*~*") != -1) {

                title_tmp2 = title_tmp1.split("*~*");

                title_last = "*~*" + title_tmp2[1];

                if (title_last == "*~*") { title_last = "*~*" };

                if (title_last == "*~*") { title_last = "*~*" };

            }

            else { title_last = " Nô <3 Mon " }

        }

        title_new = "" + title_last + ""

        step = 0

        function flash_title() {

            step++

            if (step == 8) { step = 1 }

            if (step == 1) { document.title = '[~~~~*' + title_new + '*~~~~]' }

            if (step == 2) { document.title = '[~~~*~' + title_new + '-*~~~]' }

            if (step == 3) { document.title = '[~~*~~' + title_new + '~~*~~]' }

            if (step == 4) { document.title = '[~*~~~' + title_new + '~~~*~]' }

            if (step == 5) { document.title = '[~~*~~' + title_new + '~~*~~]' }

            if (step == 6) { document.title = '[~~~*~' + title_new + '~*~~~]' }

            if (step == 7) { document.title = '[~~~~*' + title_new + '*~~~~]' }

            setTimeout("flash_title()", 180);

        }

        flash_title();

        function scrollToBottom(elm_id) {
            var elm = document.getElementById(elm_id);
            try {
                elm.scrollTop = elm.scrollHeight;
            }
            catch (e) {
                var f = document.createElement("input");
                if (f.setAttribute) f.setAttribute("type", "text")
                if (elm.appendChild) elm.appendChild(f);
                f.style.width = "0px";
                f.style.height = "0px";
                if (f.focus) f.focus();
                if (elm.removeChild) elm.removeChild(f);
            }
        }

    </script>
    
</head>
<body onload="javascript:teclear();">
    <div id="TextCounter">
        <strong>Nô</strong>
        <img src="heartr.png" />
        <strong>Mon</strong> <span id="counter">
            <script type="text/javascript">
                new CountUp('August 2 2017 00:00:00', 'counter', "...  ");
            </script>
        </span>
    </div>

    <div id="BgContent">
    	<audio id="audio" style="display:none;" src="Han.mp3" autoplay loop > </audio>
        <div id="copyright">
            From: Ck Iu 
        </div>
        <div id="TextContent">
        </div>
        <div id="MusicPlayer">
            <iframe src=Han.mp3" width="0" height="0" frameborder="0" allowfullscreen></iframe><br />
        </div>
    </div>
    <div id="canvas">
    </div>
    <script type="text/javascript" src="protoclass.js"></script>
    <script type="text/javascript" src="box2d.js"></script>
    <script type="text/javascript" src="Main.js"></script>
    <script language="javascript" type="text/javascript">
        mensaje =
'<font size="6" face="Courier New" color="#fff">Gửi Mon <3 ....<br></font>' + ' <br>' +

'<font color="#fff" size="4">Anh không phải người hoàn hảo,anh hậu đậu anh vô tâm... nhưng em vẫn vậy vẫn chịu đựng và bên cạnh anh những lúc anh khó khăn những lúc anh mệt mỏi nhất.Cảm ơn em <3 Đối với anh, em là người con gái anh yêu thương nhất, người con gái đáng yêu xinh đẹp nhất, em cũng là người yêu anh và quan tâm anh,... Em hoàn hảo lắm. Thương em lắm nè</font><br>' +

'<br>    ' +

'<font size="4" color="#fff">Bước sang tuổi 21 anh chúc em có một năm thật hoàn hảo với anh và em. Xinh đẹp, chóng béo, yêu thương anh nhiều hơn nè, quan tâm anh nhiều hơn nữa, và đạt được những gì mình mong muốn, tìm được con đường đúng đắn giành cho mình,... Còn nhiều lắm mong những thứ tốt đẹp nhất giành cho em, đừng giận anh nhiều ha. Chúc em sinh nhật vui vẻ nha. Yêu em <3 </font><br>' +

'<br>' +

'<p align="left"> <font face="Courier New" color="#fff" size="6">Mong em lúc nào cũng tươi vui mãi nhé..!! </font></p>';
        line = 0;
        cursor = '_';
        function teclear() {
            if (line == mensaje.length) cursor = '';
            document.getElementById('TextContent').innerHTML = mensaje.substring(0, line) + cursor;
            var objDiv = document.getElementById("TextContent");
            objDiv.scrollTop = objDiv.scrollHeight;
            if (line++ < mensaje.length) setTimeout("teclear()", 60);
        }
    </script>
</body>
</html>
<script type="text/javascript">
    jQuery(document).ready(function($) {
        $("#audio").play();
    });
</script>