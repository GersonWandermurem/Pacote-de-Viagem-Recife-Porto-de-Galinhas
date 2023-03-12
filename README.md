# Pacote-de-Viagem-Recife-Porto-de-Galinhas
<!DOCTYPE html>
<html>
<head>
	<title>Minha Página</title>
	<style type="text/css">
		body {
			margin: 0;
			padding: 0;
		}
		.container {
			display: flex;
			flex-direction: row;
			height: 100vh;
		}
		.side-menu {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			background-color: #f2f2f2;
			width: 200px;
			padding-top: 50px;
			position: fixed;
			top: 0;
			left: 0;
		}
		.side-menu button {
			display: block;
			width: 150px;
			height: 50px;
			background-color: #0072c6;
			color: white;
			border: none;
			border-radius: 5px;
			margin-bottom: 10px;
			font-size: 16px;
			cursor: pointer;
			box-shadow: 2px 2px 2px rgba(0, 0, 0, 0.3);
			transition: background-color 0.2s ease-in-out;
		}
		.side-menu button:hover {
			background-color: #005dac;
		}
		.side-menu button.green {
			background-color: #5cb85c;
		}
		.side-menu button.green:hover {
			background-color: #4cae4c;
		}
		.main-content {
			flex: 1;
			display: flex;
			justify-content: flex-end;
			align-items: center;
			background-color: #e6e6e6;
			padding-right: 100px;
		}
		.main-content img {
			max-width: 100%;
			max-height: 100%;
			object-fit: contain;
		}
	</style>
</head>
<body>
	<div class="container">
		<div class="side-menu">
			<button onclick="changeImage('https://drive.google.com/file/d/1lOXZnBII9H4PSzuL7eRpK5A6G5dHnW5Q/view?usp=sharing')">Tela Principal</button>
			<button onclick="changeImage('https://drive.google.com/file/d/1goDhID-I87IR7RljY5hAJh96dU65GYo_/view?usp=sharing')">Hotel - 1º Dia</button>
			<button onclick="changeImage('https://drive.google.com/file/d/1-URjDuhQ9iEs5_csHRk79mDNr42vCtdt/view?usp=sharing')">Hotel - 2º Dia</button>
			<button onclick="changeImage('https://drive.google.com/file/d/1XPQyOD2bStXPhUcAbnu9DfvHSFilk520/view?usp=sharing')">Pousada</button>
			<button class="green" onclick="window.open('https://www.reserveatlantica.com.br/hotel/costa-mar-recife-hotel-by-atlantica?letspromocode=SITEOFICIAL')">Costa Mar Recife Hotel</button>
			<button class="green" onclick="window.open('https://www.carcarapousada.com.br/')">Pousada Carcará</button>
		</div>
		<div class="main-content">
			<img id="main-image" src="https://drive.google.com/uc?id=1lOXZnBII9H4PSzuL7eRpK5A6G5dHnW5Q">
		</div>
	</div>

	<script type="text/javascript">
		function changeImage(url) {
			var image = document.getElementById("main-image");
			image.src = "https://drive.google.com/uc?id=" + url.split("/")[5];
		}
	</script>
</body>
</html>
