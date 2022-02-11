<script>
    import { link } from "svelte-routing";
</script>


<head>
	<meta name='viewport' content='width=device-width,initial-scale=1'>
	<title class="pageTitle">TumYum</title>
	<meta name="description" content="Tap into your local food scene">
	<script src="https://kit.fontawesome.com/eb06444889.js" crossorigin="anonymous"></script>
</head>
<body> 
	<div class="appInformation">
		<img class="appIcon" alt="logo" src="/build/assets/logo_rounded.png">
		<div class="appName">
			<h1>TumYum</h1>
		</div>
		<div class="appDescription">
			<p>Tap into your local food scene</p>

		</div>
		<div class="interestForm">
			<a class="typeform" href="https://za1e6wwbj28.typeform.com/to/yy4moyuj"><img class ="betaTestImg" alt="betaSignUp" src="/build/assets/beta-sign-up.png"></a>
		</div>
	</div>
	<footer>
		<section class="social">
			<div class="socialIcons">
				<a href="https://www.instagram.com/tumyumapp/"><i class="fab fa-instagram-square fa-3x"></i></a>
				<a href="https://discord.gg/75Ajsq29"><i class="fab fa-discord fa-3x"></i></a>
				<a href="https://www.youtube.com/channel/UCm0tWiLs05bMl0Lv8bkj-bw"><i class="fab fa-youtube fa-3x"></i></a>
			</div>
			<div class="privacyPolicy">
				<a href="/privacy">Privacy</a>
			</div>
		</section>
	</footer>
</body>

<style>

	*, body {
		margin: 0;
		padding: 0; 
		box-sizing: border-box;
	}

	.appInformation {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		position: relative; 
		height: 100vh;
	}

	.appInformation::before {
		content: ""; 
		background: linear-gradient(rgba(54, 59, 61, 0.8), rgba(54, 59, 61, 0.8)), url('assets/background2.jpg');
		background-repeat: no-repeat;
		background-position: center;
		background-size: cover;
		position: absolute; 
		border-radius: 0px 0px 40px 40px; 
		top: 0px; 
		right: 0px; 
		bottom: 0px; 
		left: 0px; 
		margin: 0 0 0 0; 
	}

	.appIcon {
		width: 180px;
		height: 180px;
		max-width: 100%;
		max-height: 100%;
		position: relative;
	}

	.appName {
		font-family: 'ubie';
		text-align: center;
		color: #C2EB99;
		font-size: 3rem; 
		-webkit-text-stroke: .1rem black;
		position: relative;
		margin-top: 5%;
	}

	.appDescription {
		font-family: 'playfull'; 
		text-align: center;
		color: #ecd3fa;
		font-size: 2rem; 
		position: relative;
		margin-top: 5%;
	}

	.betaTestImg {
		max-width: 75%;
		height: auto; 
		display: block; 
		margin-left: auto;
		margin-right: auto;
		position: relative;
		margin-top: 20%;
	}

	footer {
		padding-top: 2%; 
		display: flex; 
		flex-wrap: wrap;
		flex-direction: row;
		justify-content: center; 
		align-content: flex-end;
		position: relative;
	}

	.fa-instagram-square, .fa-discord, .fa-youtube {
		color: black;
	}

	.privacyPolicy {
		text-align: center; 
		font-size: 1.0rem; 
		padding-top: 3%; 
		padding-bottom: 7%;
	}

@font-face {
    font-family: 'ubie';
    src: url('/build/assets/ubie-webfont.woff') format('woff');
	font-weight: 1000;
}	

@font-face {
	font-family: 'playfull';
	src: url('/build/assets/playfull.otf') format('otf');
}

</style>