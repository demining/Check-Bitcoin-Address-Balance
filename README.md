<!DOCTYPE html>
<!-- saved from url=(0056)https://cryptodeeptech.ru/check-bitcoin-address-balance/ -->
<html lang="ru-RU"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
	
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="profile" href="https://gmpg.org/xfn/11">

	<meta name="robots" content="index, follow, max-image-preview:large, max-snippet:-1, max-video-preview:-1">

	<!-- This site is optimized with the Yoast SEO plugin v19.2 - https://yoast.com/wordpress/plugins/seo/ -->
	<style type="text/css"></style><title>How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»</title>
	<meta name="description" content="How to check Bitcoin Wallet balance using Terminal Google Colab using Python script bitcoin-checker.py convert HEX &gt; Base58">
	<link rel="canonical" href="https://cryptodeeptech.ru/check-bitcoin-address-balance/">
	<meta property="og:locale" content="ru_RU">
	<meta property="og:type" content="article">
	<meta property="og:title" content="How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»">
	<meta property="og:description" content="How to check Bitcoin Wallet balance using Terminal Google Colab using Python script bitcoin-checker.py convert HEX &gt; Base58">
	<meta property="og:url" content="https://cryptodeeptech.ru/check-bitcoin-address-balance/">
	<meta property="og:site_name" content="«CRYPTO DEEP TECH»">
	<meta property="article:published_time" content="2022-07-04T19:39:12+00:00">
	<meta property="article:modified_time" content="2022-08-25T19:17:23+00:00">
	<meta property="og:image" content="https://habrastorage.org/r/w1560/getpro/habr/upload_files/115/c50/ab8/115c50ab8b21651ae63d3cd8d3ecb98d.png">
	<meta name="author" content="Crypto Deep Tech">
	<meta name="twitter:card" content="summary_large_image">
	<meta name="twitter:label1" content="Написано автором">
	<meta name="twitter:data1" content="Crypto Deep Tech">
	<meta name="twitter:label2" content="Примерное время для чтения">
	<meta name="twitter:data2" content="5 минут">
	<script async="" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/tag.js"></script><script type="application/ld+json" class="yoast-schema-graph">{"@context":"https://schema.org","@graph":[{"@type":"WebSite","@id":"https://cryptodeeptech.ru/#website","url":"https://cryptodeeptech.ru/","name":"«CRYPTO DEEP TECH»","description":"Cryptanalysis and data financial security services","potentialAction":[{"@type":"SearchAction","target":{"@type":"EntryPoint","urlTemplate":"https://cryptodeeptech.ru/?s={search_term_string}"},"query-input":"required name=search_term_string"}],"inLanguage":"ru-RU"},{"@type":"ImageObject","inLanguage":"ru-RU","@id":"https://cryptodeeptech.ru/check-bitcoin-address-balance/#primaryimage","url":"https://habrastorage.org/r/w1560/getpro/habr/upload_files/115/c50/ab8/115c50ab8b21651ae63d3cd8d3ecb98d.png","contentUrl":"https://habrastorage.org/r/w1560/getpro/habr/upload_files/115/c50/ab8/115c50ab8b21651ae63d3cd8d3ecb98d.png"},{"@type":"WebPage","@id":"https://cryptodeeptech.ru/check-bitcoin-address-balance/#webpage","url":"https://cryptodeeptech.ru/check-bitcoin-address-balance/","name":"How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»","isPartOf":{"@id":"https://cryptodeeptech.ru/#website"},"primaryImageOfPage":{"@id":"https://cryptodeeptech.ru/check-bitcoin-address-balance/#primaryimage"},"datePublished":"2022-07-04T19:39:12+00:00","dateModified":"2022-08-25T19:17:23+00:00","author":{"@id":"https://cryptodeeptech.ru/#/schema/person/0ef8ac0f63991970628a3a6587f9e6c0"},"description":"How to check Bitcoin Wallet balance using Terminal Google Colab using Python script bitcoin-checker.py convert HEX > Base58","breadcrumb":{"@id":"https://cryptodeeptech.ru/check-bitcoin-address-balance/#breadcrumb"},"inLanguage":"ru-RU","potentialAction":[{"@type":"ReadAction","target":["https://cryptodeeptech.ru/check-bitcoin-address-balance/"]}]},{"@type":"BreadcrumbList","@id":"https://cryptodeeptech.ru/check-bitcoin-address-balance/#breadcrumb","itemListElement":[{"@type":"ListItem","position":1,"name":"Главная страница","item":"https://cryptodeeptech.ru/"},{"@type":"ListItem","position":2,"name":"How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins"}]},{"@type":"Person","@id":"https://cryptodeeptech.ru/#/schema/person/0ef8ac0f63991970628a3a6587f9e6c0","name":"Crypto Deep Tech","sameAs":["https://cryptodeeptech.ru","https://www.youtube.com/channel/UCd8W6qtRSiBn0Q0wy6HuNkQ/"],"url":"https://cryptodeeptech.ru/author/cryptodeeptech/"}]}</script>
	<!-- / Yoast SEO plugin. -->


<link rel="dns-prefetch" href="https://fonts.googleapis.com/">
<link rel="alternate" type="application/rss+xml" title="«CRYPTO DEEP TECH» » Лента" href="https://cryptodeeptech.ru/feed/">
<link rel="alternate" type="application/rss+xml" title="«CRYPTO DEEP TECH» » Лента комментариев" href="https://cryptodeeptech.ru/comments/feed/">
<link rel="stylesheet" id="itng-block-style-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_8f426a1779caff96bb3f2afbcff86bc9.css" media="all">
<link rel="stylesheet" id="wp-block-library-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/style.min.css" media="all">
<style id="global-styles-inline-css">
body{--wp--preset--color--black: #000000;--wp--preset--color--cyan-bluish-gray: #abb8c3;--wp--preset--color--white: #ffffff;--wp--preset--color--pale-pink: #f78da7;--wp--preset--color--vivid-red: #cf2e2e;--wp--preset--color--luminous-vivid-orange: #ff6900;--wp--preset--color--luminous-vivid-amber: #fcb900;--wp--preset--color--light-green-cyan: #7bdcb5;--wp--preset--color--vivid-green-cyan: #00d084;--wp--preset--color--pale-cyan-blue: #8ed1fc;--wp--preset--color--vivid-cyan-blue: #0693e3;--wp--preset--color--vivid-purple: #9b51e0;--wp--preset--gradient--vivid-cyan-blue-to-vivid-purple: linear-gradient(135deg,rgba(6,147,227,1) 0%,rgb(155,81,224) 100%);--wp--preset--gradient--light-green-cyan-to-vivid-green-cyan: linear-gradient(135deg,rgb(122,220,180) 0%,rgb(0,208,130) 100%);--wp--preset--gradient--luminous-vivid-amber-to-luminous-vivid-orange: linear-gradient(135deg,rgba(252,185,0,1) 0%,rgba(255,105,0,1) 100%);--wp--preset--gradient--luminous-vivid-orange-to-vivid-red: linear-gradient(135deg,rgba(255,105,0,1) 0%,rgb(207,46,46) 100%);--wp--preset--gradient--very-light-gray-to-cyan-bluish-gray: linear-gradient(135deg,rgb(238,238,238) 0%,rgb(169,184,195) 100%);--wp--preset--gradient--cool-to-warm-spectrum: linear-gradient(135deg,rgb(74,234,220) 0%,rgb(151,120,209) 20%,rgb(207,42,186) 40%,rgb(238,44,130) 60%,rgb(251,105,98) 80%,rgb(254,248,76) 100%);--wp--preset--gradient--blush-light-purple: linear-gradient(135deg,rgb(255,206,236) 0%,rgb(152,150,240) 100%);--wp--preset--gradient--blush-bordeaux: linear-gradient(135deg,rgb(254,205,165) 0%,rgb(254,45,45) 50%,rgb(107,0,62) 100%);--wp--preset--gradient--luminous-dusk: linear-gradient(135deg,rgb(255,203,112) 0%,rgb(199,81,192) 50%,rgb(65,88,208) 100%);--wp--preset--gradient--pale-ocean: linear-gradient(135deg,rgb(255,245,203) 0%,rgb(182,227,212) 50%,rgb(51,167,181) 100%);--wp--preset--gradient--electric-grass: linear-gradient(135deg,rgb(202,248,128) 0%,rgb(113,206,126) 100%);--wp--preset--gradient--midnight: linear-gradient(135deg,rgb(2,3,129) 0%,rgb(40,116,252) 100%);--wp--preset--duotone--dark-grayscale: url('#wp-duotone-dark-grayscale');--wp--preset--duotone--grayscale: url('#wp-duotone-grayscale');--wp--preset--duotone--purple-yellow: url('#wp-duotone-purple-yellow');--wp--preset--duotone--blue-red: url('#wp-duotone-blue-red');--wp--preset--duotone--midnight: url('#wp-duotone-midnight');--wp--preset--duotone--magenta-yellow: url('#wp-duotone-magenta-yellow');--wp--preset--duotone--purple-green: url('#wp-duotone-purple-green');--wp--preset--duotone--blue-orange: url('#wp-duotone-blue-orange');--wp--preset--font-size--small: 13px;--wp--preset--font-size--medium: 20px;--wp--preset--font-size--large: 36px;--wp--preset--font-size--x-large: 42px;}.has-black-color{color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-color{color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-color{color: var(--wp--preset--color--white) !important;}.has-pale-pink-color{color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-color{color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-color{color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-color{color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-color{color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-color{color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-color{color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-color{color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-color{color: var(--wp--preset--color--vivid-purple) !important;}.has-black-background-color{background-color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-background-color{background-color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-background-color{background-color: var(--wp--preset--color--white) !important;}.has-pale-pink-background-color{background-color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-background-color{background-color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-background-color{background-color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-background-color{background-color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-background-color{background-color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-background-color{background-color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-background-color{background-color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-background-color{background-color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-background-color{background-color: var(--wp--preset--color--vivid-purple) !important;}.has-black-border-color{border-color: var(--wp--preset--color--black) !important;}.has-cyan-bluish-gray-border-color{border-color: var(--wp--preset--color--cyan-bluish-gray) !important;}.has-white-border-color{border-color: var(--wp--preset--color--white) !important;}.has-pale-pink-border-color{border-color: var(--wp--preset--color--pale-pink) !important;}.has-vivid-red-border-color{border-color: var(--wp--preset--color--vivid-red) !important;}.has-luminous-vivid-orange-border-color{border-color: var(--wp--preset--color--luminous-vivid-orange) !important;}.has-luminous-vivid-amber-border-color{border-color: var(--wp--preset--color--luminous-vivid-amber) !important;}.has-light-green-cyan-border-color{border-color: var(--wp--preset--color--light-green-cyan) !important;}.has-vivid-green-cyan-border-color{border-color: var(--wp--preset--color--vivid-green-cyan) !important;}.has-pale-cyan-blue-border-color{border-color: var(--wp--preset--color--pale-cyan-blue) !important;}.has-vivid-cyan-blue-border-color{border-color: var(--wp--preset--color--vivid-cyan-blue) !important;}.has-vivid-purple-border-color{border-color: var(--wp--preset--color--vivid-purple) !important;}.has-vivid-cyan-blue-to-vivid-purple-gradient-background{background: var(--wp--preset--gradient--vivid-cyan-blue-to-vivid-purple) !important;}.has-light-green-cyan-to-vivid-green-cyan-gradient-background{background: var(--wp--preset--gradient--light-green-cyan-to-vivid-green-cyan) !important;}.has-luminous-vivid-amber-to-luminous-vivid-orange-gradient-background{background: var(--wp--preset--gradient--luminous-vivid-amber-to-luminous-vivid-orange) !important;}.has-luminous-vivid-orange-to-vivid-red-gradient-background{background: var(--wp--preset--gradient--luminous-vivid-orange-to-vivid-red) !important;}.has-very-light-gray-to-cyan-bluish-gray-gradient-background{background: var(--wp--preset--gradient--very-light-gray-to-cyan-bluish-gray) !important;}.has-cool-to-warm-spectrum-gradient-background{background: var(--wp--preset--gradient--cool-to-warm-spectrum) !important;}.has-blush-light-purple-gradient-background{background: var(--wp--preset--gradient--blush-light-purple) !important;}.has-blush-bordeaux-gradient-background{background: var(--wp--preset--gradient--blush-bordeaux) !important;}.has-luminous-dusk-gradient-background{background: var(--wp--preset--gradient--luminous-dusk) !important;}.has-pale-ocean-gradient-background{background: var(--wp--preset--gradient--pale-ocean) !important;}.has-electric-grass-gradient-background{background: var(--wp--preset--gradient--electric-grass) !important;}.has-midnight-gradient-background{background: var(--wp--preset--gradient--midnight) !important;}.has-small-font-size{font-size: var(--wp--preset--font-size--small) !important;}.has-medium-font-size{font-size: var(--wp--preset--font-size--medium) !important;}.has-large-font-size{font-size: var(--wp--preset--font-size--large) !important;}.has-x-large-font-size{font-size: var(--wp--preset--font-size--x-large) !important;}
</style>
<link rel="stylesheet" id="wp-date-remover-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_e6094661d8923e95b233019ebff7c8f0.css" media="all">
<link rel="stylesheet" id="itng-fonts-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/css" media="all">
<link rel="stylesheet" id="itng-style-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_8de4505c66a21eefd3c1c98b6400e4e1.css" media="all">
<link rel="stylesheet" id="itng-main-style-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_d1cf6f49400112d539e59eee9b75e10d.css" media="all">
<style id="itng-main-style-inline-css">
.custom-logo-link img {width: 400px;}@media screen and (min-width: 992px) {#header-image .header-overlay {
            opacity: 0.01;
        }}
ins,
	.nav-wrapper,
	#menu,
	.main-navigation ul#menu-desktop ul,
	#itng-featured-news .slider-post-wrapper .posted-on a,
	#itng-featured-news #itng-featured-news-list-container .posted-on a,
	#itng-featured-posts .itng-featured-post-date,
	#itng-featured-news #itng-featured-news-carousel-container .posted-on a,
	#colophon,
	[class^=itng-search] form,
	#itng-featured-cat .featured-cat-thumb h2,
	#itng-featured-cat .featured-cat-thumb h3
	{background-color: #008bca}article .entry-meta a,
	article .blog-footer,
	article .blog-footer a,
	.widget a,
	.nav-links a,
	.itng-pagination .nav-links > a,
	.itng-pagination .dots
	{color: #008bca !important}blockquote,
	#itng-content-title span
	{border-color: #008bca}button.top-menu-mobile
	{background-color: #43bdf2 !important}#footer-sidebar .widget-title
	{color: #43bdf2 !important}
</style>
<link rel="stylesheet" id="bootstrap-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_d26191bd0380b0cf97525a613b8b566c.css" media="all">
<link rel="stylesheet" id="owl-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_c8322bd5bffc8e2856f2cbcd03c61d18.css" media="all">
<link rel="stylesheet" id="mag-popup-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_30b593b71d7672658f89bfea0ab360c9.css" media="all">
<link rel="stylesheet" id="font-awesome-css" href="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_c495654869785bc3df60216616814ad1.css" media="all">
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/jquery.min.js" id="jquery-core-js"></script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/jquery-migrate.min.js" id="jquery-migrate-js"></script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_49cea0a781874a962879c2caca9bc322.js" id="wp-date-remover-js"></script>
<link rel="https://api.w.org/" href="https://cryptodeeptech.ru/wp-json/"><link rel="alternate" type="application/json" href="https://cryptodeeptech.ru/wp-json/wp/v2/posts/127"><meta name="generator" content="WordPress 6.0.1">
<link rel="alternate" type="application/json+oembed" href="https://cryptodeeptech.ru/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fcryptodeeptech.ru%2Fcheck-bitcoin-address-balance%2F">
<link rel="alternate" type="text/xml+oembed" href="https://cryptodeeptech.ru/wp-json/oembed/1.0/embed?url=https%3A%2F%2Fcryptodeeptech.ru%2Fcheck-bitcoin-address-balance%2F&amp;format=xml">
		<style type="text/css">
						#header-image {
						background-image: url(https://cryptodeeptech.ru/wp-content/uploads/2022/07/header3.jpg);
						background-size: cover;
						background-repeat: repeat;
						background-position: center center;
				}
							.site-title, .site-description {
				display: none;
				position: absolute;
				clip: rect(1px, 1px, 1px, 1px);
				}
					</style>
		<style id="custom-background-css">
body.custom-background { background-color: #eff3fd; }
</style>
	<link rel="icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-32x32.png" sizes="32x32">
<link rel="icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-192x192.png" sizes="192x192">
<link rel="apple-touch-icon" href="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-180x180.png">
<meta name="msapplication-TileImage" content="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-favicon7-270x270.png">
</head>

<body data-rsssl="1" class="post-template-default single single-post postid-127 single-format-standard custom-background wp-custom-logo no-sidebar">
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-dark-grayscale"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 0.49803921568627"></fefuncr><fefuncg type="table" tableValues="0 0.49803921568627"></fefuncg><fefuncb type="table" tableValues="0 0.49803921568627"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-grayscale"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 1"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0 1"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-purple-yellow"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.54901960784314 0.98823529411765"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0.71764705882353 0.25490196078431"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-blue-red"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 1"></fefuncr><fefuncg type="table" tableValues="0 0.27843137254902"></fefuncg><fefuncb type="table" tableValues="0.5921568627451 0.27843137254902"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-midnight"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0 0"></fefuncr><fefuncg type="table" tableValues="0 0.64705882352941"></fefuncg><fefuncb type="table" tableValues="0 1"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-magenta-yellow"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.78039215686275 1"></fefuncr><fefuncg type="table" tableValues="0 0.94901960784314"></fefuncg><fefuncb type="table" tableValues="0.35294117647059 0.47058823529412"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-purple-green"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.65098039215686 0.40392156862745"></fefuncr><fefuncg type="table" tableValues="0 1"></fefuncg><fefuncb type="table" tableValues="0.44705882352941 0.4"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 0 0" width="0" height="0" focusable="false" role="none" style="visibility: hidden; position: absolute; left: -9999px; overflow: hidden;"><defs><filter id="wp-duotone-blue-orange"><fecolormatrix color-interpolation-filters="sRGB" type="matrix" values=" .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 .299 .587 .114 0 0 "></fecolormatrix><fecomponenttransfer color-interpolation-filters="sRGB"><fefuncr type="table" tableValues="0.098039215686275 1"></fefuncr><fefuncg type="table" tableValues="0 0.66274509803922"></fefuncg><fefuncb type="table" tableValues="0.84705882352941 0.41960784313725"></fefuncb><fefunca type="table" tableValues="1 1"></fefunca></fecomponenttransfer><fecomposite in2="SourceGraphic" operator="in"></fecomposite></filter></defs></svg><div id="page" class="site">
	<a class="skip-link screen-reader-text" href="https://cryptodeeptech.ru/check-bitcoin-address-balance/#primary">Skip to content</a>

	
	    <header id="masthead" class="site-header style-1">

		    
	        <div id="header-image">
		        <div class="site-branding">
					<a href="https://cryptodeeptech.ru/" class="custom-logo-link" rel="home"><img width="1279" height="319" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/cropped-header4.png" class="custom-logo" alt="«CRYPTO DEEP TECH»" srcset="https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4.png 1279w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-300x75.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-1024x255.png 1024w, https://cryptodeeptech.ru/wp-content/uploads/2022/07/cropped-header4-768x192.png 768w" sizes="(max-width: 1279px) 100vw, 1279px" title="How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins"></a>	<h2 class="site-title"><a href="https://cryptodeeptech.ru/" rel="home">«CRYPTO DEEP TECH»</a></h2>
		<p class="site-description">Cryptanalysis and data financial security services</p>
	        	</div>
				<div class="header-overlay"></div>
	        </div>

			<div class="nav-wrapper">
				 <div class="container">
					 <div class="d-flex">

						<div id="site-navigation" class="main-navigation col-lg-11" role="navigation">
							<ul id="menu-desktop" class="menu"><li id="menu-item-229" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-229"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li id="menu-item-225" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-225"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li id="menu-item-226" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-226"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li id="menu-item-227" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-227"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li id="menu-item-228" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-228"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li id="menu-item-240" class="menu-item menu-item-type-post_type menu-item-object-post menu-item-240"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
</ul>						</div>

						<button href="#menu" class="menu-link mobile-nav-btn col-auto"><i class="fa fa-bars" aria-hidden="true"></i></button>

						<div id="search-wrapper" class="ml-auto col-auto d-flex">
							<button type="button" id="go-to-field" tabindex="-1"></button>
					    	<button class="search-btn-main"><i class="fa fa-search"></i></button>
					    	
<div class="itng-search-main">
	<form role="search" method="get" class="search-form" action="https://cryptodeeptech.ru/">
				<label>
					<span class="screen-reader-text">Найти:</span>
					<input type="search" class="search-field" placeholder="Поиск…" value="" name="s">
				</label>
				<input type="submit" class="search-submit" value="Поиск">
			</form>	<button type="button" id="go-to-btn" tabindex="-1"></button>
</div>
						</div>
					</div>
				</div>
			</div>

		</header><!-- #masthead -->
			<div id="content-wrapper" class="container row">
		
	<main id="primary" class="site-main container order-1">

		
<article id="post-127" class="post-127 post type-post status-publish format-standard hentry category-1">
	
	<header class="entry-header">
		<h1 class="entry-title">How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins</h1>	</header><!-- .entry-header -->
	
	
	
			<div class="entry-meta">
			<span class="posted-on" style="display: none;"><a href="https://cryptodeeptech.ru/check-bitcoin-address-balance/" rel="bookmark"><time class="entry-date published" datetime="" style="display: none;"></time><time class="updated" datetime=""></time></a></span><span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>		</div><!-- .entry-meta -->
		
	
	<div class="entry-content">
		<div class="entry-meta"></div>
<div class="entry-content">
<p class="has-text-align-center"><iframe title="Youtube video player" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/Hsk6QIzb7oY.html" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen" data-mce-fragment="1"></iframe></p>
<p>In this article, we will learn how to check the balance of Bitcoin coins in a large amount of data using the bitcoin-checker.py Python script for&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/bitcoin-checker.py">this&nbsp;</a><em>.</em></p>
<figure class="wp-block-image"><img title="The result of checking the Python script bitcoin-checker.py" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/115c50ab8b21651ae63d3cd8d3ecb98d.png" alt="The result of checking the Python script bitcoin-checker.py"><figcaption>The result of checking the Python script bitcoin-checker.py</figcaption></figure>
<p>We will also learn how to convert the public key of Bitcoin&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to Bitcoin Address&nbsp;&nbsp;<code>(Base58)</code>&nbsp;All this big work is done&nbsp;&nbsp;<em>by the Python script&nbsp;</em>&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/pubtoaddr.py" target="_blank" rel="noreferrer noopener">pubtoaddr.py</a></p>
<blockquote class="wp-block-quote"><p>As a result, we will check the balance of Bitcoin with particular ease by scanning the Blockchain in the Google Colab terminal&nbsp;&nbsp;<a href="https://github.com/demining/TerminalGoogleColab" target="_blank" rel="noreferrer noopener">[TerminalGoogleColab]</a></p>
<p>Earlier I recorded a video tutorial:&nbsp;&nbsp;<a href="https://www.youtube.com/watch?v=S2D7PI6dK08" target="_blank" rel="noreferrer noopener">“TERMINAL in Google Colab creating all the conveniences for working in GITHUB”</a></p></blockquote>
<p>Let’s go to the&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance" target="_blank" rel="noreferrer noopener">«CryptoDeepTools»</a>&nbsp;repository &nbsp;and take a closer look at how the&nbsp;&nbsp;<em>Bash script works:&nbsp;</em><a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/getbalance.sh" target="_blank" rel="noreferrer noopener">getbalance.sh</a></p>
<figure class="wp-block-image"><img title="Teams" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/f67caaa24e0be3727879d8c9f842f9c7.png" alt="Teams"><figcaption>Teams</figcaption></figure>
<figure class="wp-block-image"><img title="Files" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/d4557e1ae1a44f4c54e688da3a4882c7.png" alt="Files"><figcaption>Files</figcaption></figure>
<figure class="wp-block-image"><img title="Our Bash script code: getbalance.sh" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/4ff051a0999975eca9beb0b3f349896f.png" alt="Our Bash script code: getbalance.sh"><figcaption>Our Bash script code: getbalance.sh</figcaption></figure>
<pre class="wp-block-code"><code>grep 'PUBKEY = ' signatures.json &gt; pubkeyall.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>grep</code>&nbsp;collects all public keys into one common file:&nbsp;<code>pubkeyall.json</code></p>
<pre class="wp-block-code"><code>sort -u pubkeyall.json &gt; pubkey.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>sort</code>&nbsp;sorts and removes duplicates, selects unique public keys and saves the result to a file:&nbsp;<code>pubkey.json</code></p>
<pre class="wp-block-code"><code>rm pubkeyall.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>rm</code>&nbsp;removes&nbsp;<code>pubkeyall.json</code></p>
<pre class="wp-block-code"><code>sed -i 's/PUBKEY = //g' pubkey.json</code></pre>
<p>The utility&nbsp;&nbsp;<code>sed</code>&nbsp;erases the prefix&nbsp;<code>PUBKEY =</code></p>
<pre class="wp-block-code"><code>python3 pubtoaddr.py</code></pre>
<p>We&nbsp; run&nbsp;<em>the Python script&nbsp;</em>&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/pubtoaddr.py" target="_blank" rel="noreferrer noopener">pubtoaddr.py and</a>&nbsp;&nbsp;convert from the file&nbsp;&nbsp;<code>pubkey.json</code>&nbsp;where our public Bitcoin keys are stored&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to the file&nbsp;&nbsp;<code>addresses.json</code>&nbsp;the result will be saved as Bitcoin Addresses&nbsp;<code>(Base58)</code></p>
<pre class="wp-block-code"><code><strong>import</strong> hashlib
<strong>import</strong> base58
 
<strong>def</strong> <strong>hash160</strong>(hex_str):
    sha = hashlib.sha256()
    rip = hashlib.new('ripemd160')
    sha.update(hex_str)
    rip.update(sha.digest())
    <strong>return</strong> rip.hexdigest()  # .hexdigest() is hex ASCII
 
 
pub_keys = open('pubkey.json', 'r', encoding='utf-8')
new_file = open('addresses.json', 'a', encoding='utf-8')
compress_pubkey = False
 
<strong>for</strong> pub_key <strong>in</strong> pub_keys:
    pub_key = pub_key.replace('\n', '')
    <strong>if</strong> compress_pubkey:
        <strong>if</strong> (ord(bytearray.fromhex(pub_key[-2:])) % 2 == 0):
            pubkey_compressed = '02'
        <strong>else</strong>:
            pubkey_compressed = '03'
        pubkey_compressed += pub_key[2:66]
        hex_str = bytearray.fromhex(pubkey_compressed)
    <strong>else</strong>:
        hex_str = bytearray.fromhex(pub_key)
 
 
    key_hash = '00' + hash160(hex_str)
 
 
    sha = hashlib.sha256()
    sha.update(bytearray.fromhex(key_hash))
    checksum = sha.digest()
    sha = hashlib.sha256()
    sha.update(checksum)
    checksum = sha.hexdigest()[0:8]
 
#   new_file.write("" + (base58.b58encode(bytes(bytearray.fromhex(key_hash + checksum)))).decode('utf-8'))
    new_file.write((base58.b58encode(bytes(bytearray.fromhex(key_hash + checksum)))).decode('utf-8') + "\n")
pub_keys.close()
new_file.close()</code></pre>
<blockquote class="wp-block-quote"><p>We have received the file&nbsp;&nbsp;<code>addresses.json</code>&nbsp;, now we will check the balance of Bitcoin coins using the bitcoin-checker.py&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/03CheckBitcoinAddressBalance/bitcoin-checker.py" target="_blank" rel="noreferrer noopener">Python&nbsp;</a><em>script for this</em></p></blockquote>
<p>Run&nbsp;&nbsp;<em>Python script</em>&nbsp;:&nbsp;<code>python2 bitcoin-checker.py</code></p>
<pre class="wp-block-code"><code><strong>import</strong> sys
<strong>import</strong> re
<strong>from</strong> time <strong>import</strong> sleep

<strong>try</strong>:    # if is python3
    <strong>from</strong> urllib.request <strong>import</strong> urlopen
<strong>except</strong>: # if is python2
    <strong>from</strong> urllib2 <strong>import</strong> urlopen


<strong>def</strong> <strong>check_balance</strong>(address):

    #Modify the value of the variable below to False if you do not want Bell Sound when the Software finds balance.
    SONG_BELL = True

    #Add time different of 0 if you need more security on the checks
    WARN_WAIT_TIME = 0

    blockchain_tags_json = [ 
        'total_received',
        'final_balance',
        ]

    SATOSHIS_PER_BTC = 1e+8

    check_address = address

    parse_address_structure = re.match(r' *([a-zA-Z1-9]{1,34})', check_address)
    <strong>if</strong> ( parse_address_structure <strong>is</strong> <strong>not</strong> None ):
        check_address = parse_address_structure.group(1)
    <strong>else</strong>:
        print( "\nThis Bitcoin Address is invalid" + check_address )
        exit(1)

    #Read info from Blockchain about the Address
    reading_state=1
    <strong>while</strong> (reading_state):
        <strong>try</strong>:
            htmlfile = urlopen("https://blockchain.info/address/%s?format=json" % check_address, timeout = 10)
            htmltext = htmlfile.read().decode('utf-8')
            reading_state  = 0
        <strong>except</strong>:
            reading_state+=1
            print( "Checking... " + str(reading_state) )
            sleep(60*reading_state)

    print( "\nBitcoin Address = " + check_address )

    blockchain_info_array = []
    tag = ''
    <strong>try</strong>:
        <strong>for</strong> tag <strong>in</strong> blockchain_tags_json:
            blockchain_info_array.append (
                float( re.search( r'%s":(\d+),' % tag, htmltext ).group(1) ) )
    <strong>except</strong>:
        print( "Error '%s'." % tag );
        exit(1)

    <strong>for</strong> i, btc_tokens <strong>in</strong> enumerate(blockchain_info_array):

        sys.stdout.write ("%s \t= " % blockchain_tags_json[i])
        <strong>if</strong> btc_tokens &gt; 0.0:
            print( "%.8f Bitcoin" % (btc_tokens/SATOSHIS_PER_BTC) );
        <strong>else</strong>:
            print( "0 Bitcoin" );

        <strong>if</strong> (SONG_BELL <strong>and</strong> blockchain_tags_json[i] == 'final_balance' <strong>and</strong> btc_tokens &gt; 0.0): 
            
            #If you have a balance greater than 0 you will hear the bell
            sys.stdout.write ('\a\a\a')
            sys.stdout.flush()

            arq1.write("Bitcoin Address: %s" % check_address)
            arq1.write("\t Balance: %.8f Bitcoin" % (btc_tokens/SATOSHIS_PER_BTC))
            arq1.write("\n")
            arq1.close()
            <strong>if</strong> (WARN_WAIT_TIME &gt; 0):
                sleep(WARN_WAIT_TIME)

#Add the filename of your list of Bitcoin Addresses for check all.
<strong>with</strong> open("addresses.json") <strong>as</strong> file:
    <strong>for</strong> line <strong>in</strong> file:

    	arq1 = open('balance.json', 'a')
        address = str.strip(line)
        <strong>print</strong> ("__________________________________________________\n")
        
        check_balance(address)
<strong>print</strong> "__________________________________________________\n"
arq1.close()</code></pre>
<blockquote class="wp-block-quote"><p>As a result, the result will be saved in a file:&nbsp;<code>balance.json</code></p></blockquote>
<figure class="wp-block-image"><img title="File: balance.json" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/93af82c3468566ef9f495d0732c9731c.png" alt="File: balance.json"><figcaption>File: balance.json</figcaption></figure>
<h2>Now we have learned:</h2>
<ul>
<li>Convert Bitcoin Public Keys&nbsp;&nbsp;<code>PUBKEY (HEX)</code>&nbsp;to Bitcoin Address&nbsp;<code>(Base58)</code></li>
<li>Check all Bitcoin Addresses (Base58) for Bitcoin coins</li>
<li>Apply this for cryptanalysis</li>
</ul>
<p><strong>Source Code:&nbsp;&nbsp;</strong><a href="https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance" target="_blank" rel="noreferrer noopener"><strong>https://github.com/demining/CryptoDeepTools/tree/main/03CheckBitcoinAddressBalance</strong></a></p>
<p><strong>Telegram:&nbsp;&nbsp;</strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener"><strong>https://t.me/cryptodeeptech</strong></a></p>
<p><strong>Video:&nbsp;&nbsp;</strong><a href="https://youtu.be/Hsk6QIzb7oY" target="_blank" rel="noreferrer noopener"><strong>https://youtu.be/Hsk6QIzb7oY</strong></a></p>
<p><strong>Source: <a href="https://cryptodeeptech.ru/check-bitcoin-address-balance">https://cryptodeeptech.ru/check-bitcoin-address-balance</a></strong></p>
<p><iframe title="Youtube video player" src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/Hsk6QIzb7oY(1).html" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen" data-mce-fragment="1"></iframe></p>
</div>
<footer class="entry-footer">
<div class="cat-links"></div>
</footer>
	</div><!-- .entry-content -->

	<footer class="entry-footer">
		<div class="cat-links"><i class="fa fa-folder-open" aria-hidden="true"></i> <a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a></div>	</footer><!-- .entry-footer -->
</article><!-- #post-127 -->

	<nav class="navigation post-navigation" aria-label="Записи">
		<h2 class="screen-reader-text">Навигация по записям</h2>
		<div class="nav-links"><div class="nav-previous"><a href="https://cryptodeeptech.ru/break-ecdsa-cryptography/" rel="prev">The very first serious vulnerability in Blockchain and how to get the public key Bitcoin ECDSA RSZ value from the RawTX file</a></div><div class="nav-next"><a href="https://cryptodeeptech.ru/algorithms-for-secp256k/" rel="next">Useful and efficient algorithms for secp256k1 elliptic curve</a></div></div>
	</nav>		<div id="itng_related_posts_wrapper">
			<h3 id="itng_related_posts_title">Related Posts</h3>
			<div class="itng-related-posts row">
				<article id="post-372" class="itng-blog col-md-6 col-lg-4 post-372 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/shortest-ecdsa-signature/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/shortest-ecdsa-signature/">Bitcoin Wallet Recovery via ECDSA Short Signatures</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					We all know that the disclosure of the secret key in the ECDSA signature can lead to the complete recovery of the Bitcoin Wallet.&nbsp;In our earlier articles, we looked at&nbsp;weaknesses and vulnerabilities&nbsp;in blockchain transactions, but there are also ECDSA short signatures that also lead to the full recovery of a Bitcoin Wallet. Why are these ECDSA signatures…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-372 --><article id="post-112" class="itng-blog col-md-6 col-lg-4 post-112 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/break-ecdsa-cryptography/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/break-ecdsa-cryptography/">The very first serious vulnerability in Blockchain and how to get the public key Bitcoin ECDSA RSZ value from the RawTX file</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will talk about extracting signature values&nbsp;&nbsp;ECDSA R, S, Z&nbsp;​​from the Bitcoin blockchain, but first, let's remember the very first serious vulnerability in the blockchain transaction that was discovered by&nbsp;&nbsp;Niels&nbsp;Schneider&nbsp;&nbsp;(&nbsp;Nils Schneider&nbsp;aka&nbsp;&nbsp;tcatm&nbsp;&nbsp;) Bitcoin developer and owner&nbsp;&nbsp;of "BitcoinWatch"&nbsp;&nbsp;&amp;&nbsp;&nbsp;"BitcoinCharts". 4.1 History of dangerous random attacks on Bitcoin Document&nbsp;&nbsp;[PDF]:&nbsp;Private Key Recovery Combination Attacks: On Extreme Fragility of Popular…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-112 --><article id="post-97" class="itng-blog col-md-6 col-lg-4 post-97 post type-post status-publish format-standard hentry category-1">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/blockchain-google-drive/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/blockchain-google-drive/">How to Parse Blockchain Transactions to a Google Drive Folder</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will analyze bitcoin transactions and learn how to parse RawTX very quickly from the blockchain network to the Google Drive folder, all this will help us better understand how bitcoin transactions work and what all its contents are on the blockchain network. First, we need to know that all bitcoin transactions are stored…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/%d0%b1%d0%b5%d0%b7-%d1%80%d1%83%d0%b1%d1%80%d0%b8%d0%ba%d0%b8/" rel="category tag">Без рубрики</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-97 -->			</div>
		</div>
			<div id="author_box" class="row no-gutters">
			<div class="author_avatar col-2">
							</div>
			<div class="author_info col-10">
				<h4 class="author_name title-font">
					Crypto Deep Tech				</h4>
				<div class="author_bio">
									</div>
			</div>
		</div>
	
	</main><!-- #main -->

<!--WCLEARFY_PAGE_TYPE_post--><!--WCLEARFY_FOOTER_START--></div><!-- #content-wrapper -->


 <div id="footer-sidebar" class="widget-area">
    <div class="container">
        <div class="row">
                    </div>
    </div>
</div>
	<footer id="colophon" class="site-footer">
		<div class="container">
			<div class="site-info">
				Donation Address: <a href="https://www.blockchain.com/btc/address/1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v" target="_blank">♥  BTC: 1Lw2kh9WzCActXSGHxyypGLkqQZfxDpw8v</a>				<span class="sep"> | </span>
					Copyright © 2022 «CRYPTO DEEP TECH». 			</div><!-- .site-info -->
		</div>
	</footer><!-- #colophon -->
</div><!-- #page -->

<nav id="menu" class="panel" role="navigation" style="position: fixed; top: 0px; bottom: 0px; height: 100%; left: -15.625em; width: 15.625em;">
	<div class="menu-overlay"></div>
	<div id="panel-top-bar">
		<button class="go-to-bottom"></button>
		<button id="close-menu" class="menu-link"><i class="fa fa-chevron-left" aria-hidden="true"></i></button>
	</div>

	<ul id="menu-main" class="menu"><li class="page_item page-item-53"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li class="page_item page-item-43"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li class="page_item page-item-55"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li class="page_item page-item-49"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
</ul>

	<button class="go-to-top"></button>
</nav>

<div id="sticky-navigation">
	<div class="nav-wrapper">
		 <div class="container">

			 <div class="row justify-content-end align-items-center justify-content-between no-gutters">


				<div class="main-navigation col-lg-9" role="navigation">
					<ul id="menu-desktop" class="menu"><li class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-229"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-225"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-226"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-227"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-228"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-post menu-item-240"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
</ul>				</div>

				<button href="#menu" class="menu-link mobile-nav-btn"><i class="fa fa-bars" aria-hidden="true"></i></button>

				<button type="button" id="go-to-field" tabindex="-1"></button>

				<button class="search-btn-sticky ml-auto col-auto"><i class="fa fa-search"></i></button>
				
<div class="itng-search-sticky">
	<form role="search" method="get" class="search-form" action="https://cryptodeeptech.ru/">
				<label>
					<span class="screen-reader-text">Найти:</span>
					<input type="search" class="search-field" placeholder="Поиск…" value="" name="s">
				</label>
				<input type="submit" class="search-submit" value="Поиск">
			</form>	<button type="button" id="go-to-btn" tabindex="-1"></button>
</div>

			</div>
		</div>
	</div>
</div>

<div id="itng-back-to-top" class="show"><i class="fa fa-chevron-up" aria-hidden="true"></i></div>

		<script type="text/javascript">
							jQuery("#post-127 .entry-meta .date").css("display","none");
					jQuery("#post-127 .entry-date").css("display","none");
					jQuery("#post-127 .posted-on").css("display","none");
							jQuery("#post-372 .entry-meta .date").css("display","none");
					jQuery("#post-372 .entry-date").css("display","none");
					jQuery("#post-372 .posted-on").css("display","none");
							jQuery("#post-112 .entry-meta .date").css("display","none");
					jQuery("#post-112 .entry-date").css("display","none");
					jQuery("#post-112 .posted-on").css("display","none");
							jQuery("#post-97 .entry-meta .date").css("display","none");
					jQuery("#post-97 .entry-date").css("display","none");
					jQuery("#post-97 .posted-on").css("display","none");
				</script>
	<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_2b1ae4cca3cc8d12c39be42768565308.js" id="big-slide-js"></script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_ccdf893e7d8b26933af0c336bcc3943e.js" id="owl-js-js"></script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/jquery.magnific-popup.min.js" id="mag-lightbox-js-js"></script>
<script id="itng-custom-js-js-extra">
var itng = {"toTopEnable":"1","stickyNav":""};
</script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_ea8874ba65dbd53bf5c7fb5c619ac579.js" id="itng-custom-js-js"></script>
<script src="./How to Convert Bitcoin-PUBKEY HEX Public Keys to Base58 Bitcoin Address and Check Balance for BTC Coins - «CRYPTO DEEP TECH»_files/wmac_single_6ec0e9b3201c83a442e24aba829a5f05.js" id="itng-navigation-js"></script>
<!-- Yandex.Metrika counter --> <script type="text/javascript"> (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)}; m[i].l=1*new Date();k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)}) (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym"); ym(89424273, "init", {  id:89424273, clickmap:true, trackLinks:true, webvisor:true, accurateTrackBounce:true }); </script> <noscript><div><img src="https://mc.yandex.ru/watch/89424273" style="position:absolute; left:-9999px;" alt="" /></div></noscript> <!-- /Yandex.Metrika counter -->
<!-- Yandex.Metrika counter -->
<script type="text/javascript">
   (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
   var z = null;m[i].l=1*new Date();
   for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
   k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)})
   (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");

   ym(89995532, "init", {
        clickmap:true,
        trackLinks:true,
        accurateTrackBounce:true,
        webvisor:true
   });
</script>
<noscript><div><img src="https://mc.yandex.ru/watch/89995532" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter -->


</body></html>