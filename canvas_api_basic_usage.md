https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage

#`CANVAS` НЕГІЗГІ ПАЙДАЛАНУ ЖОЛДАРЫ

##`<canvas>` ЭЛЕМЕНТІ
	
Бұл оқулықты ең бірінші <canvas> элементіне қараудан бастайық.

	1 <canvas id="tutorial" width="150" height="150"></canvas>
	
Бір қарағанда `<img>` элементіне өте қатты ұқсайды, тек айырмашылығы `src` және `alt` атрибуттарының жоқтығында. `<canvas>` элементінде тек екі-ақ атрибут бар - `width` және `height`. Ол екеуі де міндетті атрибуттарға жатпайды, оларды басқаша `DOM` -ның қасиеттері арқылы тағайындауға да болады. `Canvas` элементінде `width` және `height` атрибуттары көрсетілмеген жағдайда бастапқы мәндері сәйкесінше `300 px` және `150 px` деп алынады. Элементтің өлшемдеін `CSS` арқылы қалауыңызша өзгерте аласыз, бірақ сурет қайта сызылған кезде сол жаңа өлшемдерге сиятындай етіп сызылады.
	
> ЕСКЕРТУ: егер сызылған кезде пропорциясы өзгеріске ұшырайтын болса, онда `width` және `height` атрибуттарын нақтылай және `CSS` -ты пайдаланбай өзгертіңіз.
	
`id` атрибуты `<canvas>` элементінің спецификациясы емес, бірақ әрбір `HTML` элементтеріне тән бастапқы атрибуттардың (мысалыға `class` сияқты) бірі болғандықтан пайдаланылады. `id` -ды әрқашанда пайдаланып отыру жақсы әдетке саналады, өйткені бұлай белгілеу сізге `javascript` -те кейін оны оңай табуға мүмкіндік береді.
	
Кез келген кәдімгі суреттердегі секілді `<canvas>` элементіне де стильдерді (`margin`, `border` т.с.с) қолдануға болады. Дегенменде бұл ережелер `canvas` -тың ішіндегі суреттерге әсер етпейді. Кейіндеу осы оқулықта мұның қалай болатынын көретін боламыз. Стильдегі ережелер қолданылмаған жағдайда `canvas` -тың фоны әдетте толықтай мөлдір болып сызылады.
	
##FALLBACK CONTENT (ОРАҒЫТЫП ӨТУ КОНТЕКСТІ)
	
Кейбір ескі браузерлерде (әсіресе `Internet Explorer` 9 нұсқасынан бұрынғылар) `<canvas>` элементін түсінбейтін болғандықтан сізге мұны айналып өтудің басқа жолын іздеуге тура келеді. 
	
Ең тура жолы: `<canvas>` элементінің ішіндегілерді альтернативті жолмен басқаша жасаймыз. `<canvas>` -ты түсінбейтін басқа браузерлер оны елеместен альтернативті жолымен сызуға кіріседі.
	
Мысал үшін, `canvas` -ты сипаттайтын мәтін жазамыз немесе динамикалы түрде сызылатын статикалық суреттерді тығамыз. Солардың бірі мынау, қарап көріңіз:

	1 <canvas id="stockGraph" width="150" height="150">
	2   current stock price: $3.15 +0.15
	3 </canvas>
	4 
	5 <canvas id="clock" width="150" height="150">
	6   <img src="images/clock.png" width="150" height="150" alt=""/>
	7 </canvas>
	
##`</CANVAS>` ТЕГІ МІНДЕТТІ
	
`img` элементінен айырмашылығы `<canvas>` элементіне міндетті түрде жабатын тег `</canvas>` қажет. Егер орағытып өтудің қажеті болмаса, онда жай ғана былай жазыңыз: `<canvas id="foo" ...></canvas>`, мұны `canvas` -пен жұмыс істейтін барлық браузерлер түсінеді.
	
	
