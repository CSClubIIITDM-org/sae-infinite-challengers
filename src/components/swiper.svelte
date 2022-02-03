<script>
	import { Swiper, SwiperSlide } from 'swiper/svelte';
	import { EffectCoverflow, Keyboard, Mousewheel } from 'swiper';
	import 'swiper/css';
	import 'swiper/css/effect-coverflow';
	$: innerWidth = 0;
</script>

<svelte:window bind:innerWidth />
<section>
	<Swiper
		modules={[Keyboard, EffectCoverflow, Mousewheel]}
		spaceBetween={10}
		slidesPerView={3}
		loop={true}
		centeredSlides={true}
		effect="coverflow"
		mousewheel={{
			invert: false
		}}
		coverflowEffect={{
			slideShadows: false
		}}
		keyboard
	>
		{#each Array(6) as _, i}
			<SwiperSlide>
				<div class="slide">
					<img src="./teams/teamposts/{i + 1}.png" alt="team-post" />
				</div>
			</SwiperSlide>
		{/each}
	</Swiper>
</section>

<style>
	section {
		margin: 100px 0;
	}
	.slide img {
		height: 350px;
		user-select: none;
		-moz-user-select: none;
		-webkit-user-drag: none;
		-webkit-user-select: none;
		-ms-user-select: none;
	}
	@media (max-width: 1200px) {
		.slide img {
			height: 250px;
		}
	}
	@media (max-width: 768px) {
		section {
			margin: 50px 0;
		}
		.slide img {
			height: 175px;
		}
	}
	@media (max-width: 520px) {
		.slide img {
			height: 130px;
		}
	}
	@media (max-width: 400px) {
		.slide img {
			height: 100px;
		}
	}
</style>
