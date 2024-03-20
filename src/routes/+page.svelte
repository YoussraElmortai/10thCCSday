<script>
</script>

<div class="bob"></div>
<div class="bobs"></div>

<main class="container"></main>

<style>
	.bob {
		background: linear-gradient(to right, rgb(0, 255, 149), purple, rgb(194, 52, 182));

		height: 25rem;
		width: 25rem;
		opacity: 40%;
		position: absolute;
		z-index: 2;
		animation: rotate 20s infinite;
		filter: blur(5rem);
	}
	.bobs {
		background: linear-gradient(to right, rgb(52, 0, 242), rgb(0, 128, 19), indigo);
		left: 55%;
		top: 13%;
		height: 25rem;
		width: 25rem;
		opacity: 45%;
		position: absolute;
		z-index: 2;
		animation: rotate 20s infinite;
		filter: blur(5rem);
	}

	@keyframes rotate {
		from {
			transform: rotate(0deg);
		}
		50% {
			transform: scale(1, 1.2);
		}
		to {
			transform: rotate(360deg);
		}
	}

	.container {
		filter: url(#grainy);
		height: 100%;
		width: 100vw;
		position: absolute;
		top: 0;
		left: 0;
		border-radius: 50%;
		opacity: 50%;
		overflow: hidden;
	}
</style>
