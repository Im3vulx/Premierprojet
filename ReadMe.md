<h1>Hey je m'appelle Loïc HUET</h1>

<header class="header">
	<h1 class="glitched">Glitch</h1>
</header>
<a class="inspiration-button" href="http://www.theverge.com/a/luka-artificial-intelligence-memorial-roman-mazurenko-bot" target="_blank">Inspiration</a>

<stlye>$background-color: #F9F8F8;
$headline-color: #222222;
*{
	box-sizing: border-box;
}
body{
	font-family: 'Raleway', sans-serif;
	background: $background-color;
}
header.header{
	position: absolute;
	top: 50%;
	left: 0;
	width: 100%;
	transform: translateY(-50%);
	h1{
		font-size: 8rem;
		color: $headline-color;
		text-align: center;
		margin-top: 0;
		text-transform: uppercase;
		font-weight: 900;
	}
}
.glitch-window{
	position: absolute;
	top: 0;
	left: -2px;
	width: 100%;
	color: $headline-color;
	text-shadow: 2px 0 $background-color, -1px 0 yellow, -2px 0 green;
	overflow: hidden;
	animation: crt-me 2500ms infinite linear alternate-reverse;
	// background: red;
}

//Animation Keyframes
@keyframes crt-me {
	 0% {
        clip: rect(31px, 9999px, 94px, 0)
    }
    10% {
        clip: rect(112px, 9999px, 76px, 0)
    }
    20% {
        clip: rect(85px, 9999px, 77px, 0)
    }
    30% {
        clip: rect(27px, 9999px, 97px, 0)
    }
    40% {
        clip: rect(64px, 9999px, 98px, 0)
    }
    50% {
        clip: rect(61px, 9999px, 85px, 0)
    }
    60% {
        clip: rect(99px, 9999px, 114px, 0)
    }
    70% {
        clip: rect(34px, 9999px, 115px, 0)
    }
    80% {
        clip: rect(98px, 9999px, 129px, 0)
    }
    90% {
        clip: rect(43px, 9999px, 96px, 0)
    }
    100% {
        clip: rect(82px, 9999px, 64px, 0)
    }
    
}



//Inspiration Button
.inspiration-button{
	font-family: Helvetica, sans-serif;
	position: fixed;
	display: inline-block;
	z-index: 100;
	bottom: 1rem;
	left: 50%;
	transform: translate(-50%, 0%);
	color: white;
	text-decoration: none;
	padding: 0.75rem 1rem;
	border-radius: 80px;
	background: linear-gradient(270deg,#1e80dc,#c61590);
	//From Instagram...thanks
	transition: transform 250ms ease;
	&:hover, &:focus, &:active{
		transform: translate(-50%, -10%);

	}
}
</style>

<script type="text/javascript">$("header").append("<div class='glitch-window'></div>");
//fill div with clone of real header
$( "h1.glitched" ).clone().appendTo( ".glitch-window" );
</script>