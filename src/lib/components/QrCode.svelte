<script lang="ts">
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
	@use '$lib/styles/variables' as *;

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
