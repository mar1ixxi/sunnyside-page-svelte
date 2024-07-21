<script>
	import logo from '$lib/images/logo.svg';
	import down_arrow from '$lib/images/icon-arrow-down.svg';
	import main_bg from '$lib/images/desktop/image-header.jpg';
	import egg_bg from '$lib/images/desktop/image-transform.jpg'
	import cup from '$lib/images/desktop/image-stand-out.jpg';
	import cherry from '$lib/images/desktop/image-graphic-design.jpg';
	import orange from '$lib/images/desktop/image-photography.jpg';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Sunnyside Landing Page" />
</svelte:head>

<section class="bg-white w-full h-auto flex flex-col items-center justify-center relative">

	<div class="w-full min-h-screen h-full flex flex-col gap-20 items-center justify-center relative">

		<nav class="flex flex-row justify-between absolute top-4 w-full h-auto px-12 py-2">
			<img src={logo} alt="" class=" w-auto h-8">
			<div class="font-barlow font-semibold text-white text-base flex gap-12 items-center justify-center">
				<span class="cursor-pointer">About</span>
				<span class="cursor-pointer">Services</span>
				<span class="cursor-pointer">Projects</span>
				<span class="py-3 px-6 rounded-full bg-white text-black font-fraunces uppercase cursor-pointer">Contact</span>
			</div>
		</nav>

		<div class="absolute flex flex-col gap-20 items-center top-1/3">
			<h3 class="md:text-6xl text-3xl text-white font-black tracking-wider font-fraunces uppercase">We are creatives</h3>
			<img src={down_arrow} alt="" class="w-8 h-auto" />
		</div>
		<img src={main_bg} alt="" class="w-full h-full object-cover">

	</div>

	<div class="w-full h-auto flex flex-col">
		<div class="flex flex-row w-full h-auto">
			<div class="w-1/2 h-auto">
				<div>Transform your brand</div>
				<div>
					We are a full-service creative agency specializing in helping brands grow fast. 
					Engage your clients through compelling visuals that do most of the marketing for you.
				</div>
				<button>Learn more</button>
			</div>
			<img src={egg_bg} alt="" class="w-1/2 h-full" />
		</div>
	</div>

	<div class="w-full h-auto flex flex-col">
		<div class="flex flex-row w-full h-auto">
			<img src={cup} alt="" class="w-1/2 h-full" />
			<div class="w-1/2 h-auto">
				<div>Stand out to the right audience</div>
				<div>
					Using a collaborative formula of designers, researchers, photographers, videographers, and copywriters, we’ll build and extend your brand in digital places.
				</div>
				<button>Learn more</button>
			</div>
		</div>
	</div>

	<div class="w-full h-auto flex flex-col">
		<div class="flex flex-row w-full h-auto">
			<div class="w-1/2 h-full bg-cherry">
				<img src={cherry} alt="" class="w-full h-full" />
				<div>
					<span>Graphic design</span>
					<span>Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention.</span>
				</div>
			</div>
			<div class="w-1/2 h-full bg-orange">
				<img src={orange} alt="" class="w-full h-full" />
				<div>
					<span>Photography</span>
					<span>Increase your credibility by getting the most stunning, high-quality photos that improve your business image.</span>
				</div>
			</div>
		</div>
	</div>

	<div class="flex flex-col">
		<h3>Client testimonials</h3>

		<div class="flex flex-row gap-8">
			<div>
				<img src="" alt="">
				<div>We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</div>
				<div>
					<span>Emily R.</span>
					<span>Marketing Director</span>
				</div>
			</div>
	
			<div>
				<img src="" alt="">
				<div>Sunnyside’s enthusiasm coupled with their keen interest in our brand’s success made it a satisfying and enjoyable experience.</div>
				<div>
					<span>Thomas S.</span>
					<span>Chief Operating Officer</span>
				</div>
			</div>
	
			<div>
				<img src="" alt="">
				<div>Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!</div>
				<div>
					<span>Jennie F.</span>
					<span>Business Owner</span>
				</div>
			</div>
		</div>

	</div>

	<div>
		<img src="" alt="">
		<div>
			<span></span>
			<span></span>
			<span></span>
		</div>
		<div>
			<img src="" alt="">
			<img src="" alt="">
			<img src="" alt="">
			<img src="" alt="">
		</div>
	</div>

</section>