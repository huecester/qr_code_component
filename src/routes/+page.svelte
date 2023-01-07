<script lang="ts">
	import '@fontsource/outfit/400.css';
	import '@fontsource/outfit/700.css';
	import 'normalize.css/normalize.css';

	import qrCode from '$lib/images/qr_code.png';
</script>

<div class="card">
	<img src={qrCode} alt="QR Code for Frontend Mentor" />
	<section class="card-text">
		<h1>Improve your front-end skills by building projects</h1>
		<p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
	</section>
</div>

<style lang="scss">
	$clr-primary-main: hsl(218, 44%, 22%);
	$clr-primary-sub: hsl(220, 15%, 55%);

	$clr-background-card: hsl(0, 0%, 100%);
	$clr-background-page: hsl(212, 45%, 89%);

	$ff-primary: 'Outfit', sans-serif;

	$fw-bold: 700;
	$fw-normal: 400;

	$fs-header: 1.5rem;
	$fs-primary: 1rem;

	:global(*) {
		box-sizing: border-box;
		font: inherit;
	}

	:global(body) {
		font-family: $ff-primary;
		background-color: $clr-background-page;
		height: 100vh;

		display: flex;
		align-items: center;
		justify-content: center;
	}

	.card {
		display: flex;
		flex-direction: column;

		width: 22rem;
		padding: 1.25rem;
		border-radius: 1.25rem;

		background-color: $clr-background-card;

		img {
			border-radius: 0.75rem;
		}

		.card-text {
			margin: 1rem;

			h1 {
				color: $clr-primary-main;
				font-weight: $fw-bold;
				font-size: $fs-header;
				text-align: center;
			}

			p {
				color: $clr-primary-sub;
				font-weight: $fw-normal;
				font-size: $fs-primary;
				text-align: center;
			}
		}
	}
</style>
