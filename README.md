# Mario
Mario feito com HTML + CSS + JAVASCRIPT

HTML <!-- Cada linha dessas vai representar um pixel do desenho do Mário

w = White
r = Red
b = Brown
y = Yellow
o = Orange

j = Pula para a próxima linha

-->
<div id="whoIs">
		wwwrrrrrwwwwj
		wwrrrrrrrrrwj
		wwbbboobowwwj
		wbobooobooowj
		wbobboooboooj
		wbboooobbbbwj
		wwwoooooowwwj
		wwbbrbbbwwwwj
		wbbbrbbrbbbwj
		bbbbrrrrbbbbj
		oobryrryrbooj
		ooorrrrrroooj
		oorrrrrrrrooj
		wwrrrwwrrrwwj
		wbbbwwwwbbbwj
		bbbbwwwwbbbbj
	</div>
    
    CSS
    
    /* O Css é responsável por dar o estilo de cada pixel(div) após as letras serem subistituídas através do Java Script*/

.w,.r,.b,.o,.y{
			display: inline-block;
			width: 50px;
			height: 50px;
			margin-top:-4px;
		}
		.w{
			background: white;
		}
		.r{
			background: #FB0405;
		}
		.o{
			background: #FF9F10;
		}
		.b{
			background: #7D5307;
		}
		.y{
			background: #F6A412;
		}
        
    

JAVASCRIP
</div><div class='r'></div><div class='r'></div><div class='w'></div><div class='w'></div><div class='w'></div><div class='w'></div><br>
    
    let str = document.getElementById("whoIs").innerHTML;
			    str = str.replace(/w/g, "<div class='w'></div>");
			    str = str.replace(/r/g, "<div class='r'></div>");
			    str = str.replace(/o/g, "<div class='o'></div>");
			    str = str.replace(/b/g, "<div class='b'></div>");
			    str = str.replace(/y/g, "<div class='y'></div>");
			    str = str.replace(/j/g, "<br>");


			document.getElementById("whoIs").innerHTML = str;

		