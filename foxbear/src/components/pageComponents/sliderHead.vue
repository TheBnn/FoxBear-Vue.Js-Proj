<template>
	<div class="slider">
		<div class="slider_slide">
			<img src="@/assets/imgs/1920x793slider.png">
			<div class="slide_container">
				<div class="slide_title">Кейтеринг</div>
				<div class="slide_info">
					<div class="info_text">Есть много вариантов Lorem Ipsum, но большинство из них имеет не всегда
						приемлемые модификации</div>
					<div class="info_button">
						<button class="button">Подробнее</button>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'sliderHead',
		props: {

		}
	}
</script>

<style>
	.slider img {
		z-index: -1;
		max-width: 100%;
		max-height: 100%;
		height: 100%;
		width: 100%;
	}

	.slider .slider_slide {
		position: relative;
		z-index: 1;
		padding: 0;
		margin: 0;
		line-height: 0;
	}

	.slider .slider_slide .slide_container {
		font-family: 'Gotham Pro';
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		position: absolute;
		top: 0;
		bottom: 0;
		right: 0;
		left: 0;
		color: white;
	}

	.slider .slider_slide .slide_container .slide_info {
		width: 65%;
	}

	.slider .slider_slide .slide_container .info_button {
		display: flex;
		justify-content: center;
	}

	.slider .slider_slide .slide_container .slide_title {
		font-size: 99px;
		font-weight: bold;
		line-height: 1;
		padding-bottom: 30px;
	}

	.slider .slider_slide .slide_container .slide_info .info_text {
		margin: 0 auto;
		font-size: 30px;
		line-height: 33px;
		text-align: center;
		padding-bottom: 33px;
	}

	.info_button .button {
		border: none;
		font-size: 22px;
		line-height: 33px;
		border-radius: 33px;
		width: 252px;
		height: 65px;
		color: white;
		background: linear-gradient(45deg, #D97943, #9A4617);
	}
</style>