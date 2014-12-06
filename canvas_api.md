#https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API

##Canvas

HTML5 -ке қосылған <canvas> HTML элементімен Javascript арқылы түрлі графиктер салуға болады. Мысал үшін, онымен графиктер, фото композициялар, анимациялар немесе керек болса real-time режимде видеоларды өңдеуге немесе жасауға болады.

Mozilla applications ұжымы Gecko 1.8 ядросында <canvas> -ты дамытуға көптеген үлес қосып жатыр (мысалы Firefox 1.5). Бұл элемент алғашқы рет Apple компаниясының бастамасымен OS X Dashboard және Safari бағдарламаларында енгілізілді. Internet Explorer -де <canvas> 9 нұсқасынан бастап қолданысқа енгізілді. Google -дың Explorer Canvas жобасынның кодтарын пайдаланудың арқасында Internet Explorer -дің алдыңғы нұсқаларында да <canvas> тиімді жұмыс жасай бастады. Opera 9 және Google Chrome браузерлерінде <canvas> элементін қолдануға болады.

Бұл <canvas> элементі ғаламтор беттерінде 3D графикалар салуды аппаратты жолмен жылдамдату мақсатында WebGL -де де пайдаланылады.

##МЫСАЛ

CanvasRenderingContext2D.fillRect() методы пайдаланылған жай қарапайым ғана кодтан үзінді:

HTML
     1 <canvas id="canvas"></canvas>

JavaScript
     1 var canvas = document.getElementById("canvas");
     2 var ctx = canvas.getContext("2d");
     3 
     4 ctx.fillStyle = "green";
     5 ctx.fillRect(10, 10, 100, 100);
		
Төмендегі кодты өзгерту арқылы canvas элементіндегі өзгерісті сол сәтте бақылап көре аласыз	

	СІЛТЕМЕЛЕР

		HTMLCanvasElement
		CanvasRenderingContext2D
		CanvasGradient
		CanvasPattern
		ImageData
		TextMetrics
		Path2D 
		WebGLRenderingContext -ке қатысты интерфейстер мына жерден қарай аласыз https://developer.mozilla.org/en-US/docs/Web/WebGL
		
	ОҚУЛЫҚТАР МЕН НҰСҚАУЛАР
	
		Canvas оқулығы https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial
			<canvas> элементін пайдаланудың негізі және қосымша мүмкіншіліктері жайлы комплексті оқулық
			
		Кодтардан үзінділер: Canvas https://developer.mozilla.org/en-US/Add-ons/Code_snippets/Canvas
			Бардарламашыларға арналған қосымшалардан <canvas> -қа байланысты кодтардардың үзінділері
			
		Демо: A basic raycaster https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/A_basic_ray-caster
			A demo of ray-tracing animation using canvas.
			
		Canvas элементінің ішінде DOM объектілерін салу https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Drawing_DOM_objects_into_a_canvas
			Canvas элементінің ішінде DOM объектілерін салу
			
		canvas -ты пайдаланып графиктер салу https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Drawing_graphics_with_canvas
			Canvas жайлы ескі кіріспе беттер Canvas оқулығының беттерімен алмастырылған
			
		
		РЕСУРСТАР
		Негізгілері
			HTML5 Canvas Deep Dive http://joshondesign.com/p/books/canvasdeepdive/title.html
			Canvas cheat sheet (PNG / PDF) http://blog.nihilogic.dk/2009/02/html5-canvas-cheat-sheet.html
			Canvas Handbook http://bucephalus.org/text/CanvasHandbook/CanvasHandbook.html
			
		Libraries
			Fabric.js is an open-source canvas library with SVG parsing capabilities 
			Kinetic.js is an open-source canvas library focused on interactivity for desktop and mobile applications
			Paper.js is an open source vector graphics scripting framework that runs on top of the HTML5 Canvas
			libCanvas is powerful and lightweight canvas framework
			Processing.js is a port of the Processing visualization language
			EaselJS is a library with a Flash-like API
			PlotKit is a charting and graphing library
			Rekapi is an animation key-framing API for Canvas
			PhiloGL is a WebGL framework for data visualization, creative coding and game development.
			JavaScript InfoVis Toolkit creates interactive 2D Canvas data visualizations for the Web.
			Frame-Engine is a framework for developing applications and games
			
		СПЕЦИФИКАЦИЯ
		
			Спецификация	                                             Статусы	          Түсіндірме
			WHATWG HTML Living Standard	                               Living Standard
			The definition of 'Canvas' in that specification.
			https://html.spec.whatwg.org/multipage/the-canvas-element.html
			
		СОНЫМЕН ҚАТАР
			
			WebGL
