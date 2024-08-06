<script>
	import logo from '$lib/images/logo.svg';
	import down_arrow from '$lib/images/icon-arrow-down.svg';
	import main_bg from '$lib/images/desktop/image-header.jpg';
	import egg_bg from '$lib/images/desktop/image-transform.jpg'
	import cup from '$lib/images/desktop/image-stand-out.jpg';
	import cherry from '$lib/images/desktop/image-graphic-design.jpg';
	import orange from '$lib/images/desktop/image-photography.jpg';

	import firstPerson from '$lib/images/image-emily.jpg';
	import secondPerson from '$lib/images/image-jennie.jpg';
	import thirdPerson from '$lib/images/image-thomas.jpg';

	import milkBottles from '$lib/images/desktop/image-gallery-milkbottles.jpg'
	import orangeSecond from '$lib/images/desktop/image-gallery-orange.jpg'
	import conesSecond from '$lib/images/desktop/image-gallery-cone.jpg'
	import sugarCubes from '$lib/images/desktop/image-gallery-sugarcubes.jpg'

	import facebook from '$lib/images/icon-facebook.svg'
	import instagram from '$lib/images/icon-instagram.svg'
	import pinterest from '$lib/images/icon-pinterest.svg'
	import twitter from '$lib/images/icon-twitter.svg'
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

	<div class="w-full h-auto flex flex-col font-fraunces">
		<div class="flex flex-row w-full h-auto">
			<div class="w-1/2 h-auto p-40 flex flex-col items-start gap-6">
				<div class="text-4xl font-bold text-black">Transform your brand</div>
				<div class='font-barlow text-lg'>
					We are a full-service creative agency specializing in helping brands grow fast. 
					Engage your clients through compelling visuals that do most of the marketing for you.
				</div>
				<button class="uppercase">Learn more</button>
			</div>
			<img src={egg_bg} alt="" class="w-1/2 h-full" />
		</div>
	</div>

	<div class="w-full h-auto flex flex-col font-fraunces">
		<div class="flex flex-row w-full h-auto">
			<img src={cup} alt="" class="w-1/2 h-full" />
			<div class="w-1/2 h-auto p-40 flex flex-col items-start gap-6">
				<div class="text-4xl font-bold text-black">Stand out to the right audience</div>
				<div class="font-barlow text-lg">
					Using a collaborative formula of designers, researchers, photographers, videographers, and copywriters, we’ll build and extend your brand in digital places.
				</div>
				<button class="uppercase">Learn more</button>
			</div>
		</div>
	</div>

	<div class="w-full h-auto flex flex-col">
		<div class="flex flex-row w-full h-auto">
			<div class="w-1/2 h-full bg-cherry relative flex items-center justify-center">
				<img src={cherry} alt="" class="w-full h-full" />
				<div class='absolute bottom-10 flex flex-col items-center justify-center gap-4 md:w-2/3 w-11/12'>
					<span class="text-4xl font-bold text-black font-fraunces">Graphic design</span>
					<span class="font-barlow text-lg text-center">Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention.</span>
				</div>
			</div>
			<div class="w-1/2 h-full bg-orange relative flex items-center justify-center">
				<img src={orange} alt="" class="w-full h-full" />
				<div class='absolute bottom-10 flex flex-col items-center justify-center gap-4 md:w-2/3 w-11/12'>
					<span class="text-4xl font-bold text-black font-fraunces">Photography</span>
					<span class="font-barlow text-lg text-center">Increase your credibility by getting the most stunning, high-quality photos that improve your business image.</span>
				</div>
			</div>
		</div>
	</div>

	<div class="flex flex-col md:w-10/12 w-11/12 h-auto py-10 gap-20 items-center justify-center">
		<h3 class="text-2xl font-fraunces uppercase">Client testimonials</h3>

		<div class="flex flex-row gap-8">
			<div class="flex flex-col gap-8 items-center">
				<img src={firstPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center">We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces">Emily R.</span>
					<span>Marketing Director</span>
				</div>
			</div>
	
			<div class="flex flex-col gap-8 items-center">
				<img src={secondPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center">Sunnyside’s enthusiasm coupled with their keen interest in our brand’s success made it a satisfying and enjoyable experience.</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces">Thomas S.</span>
					<span>Chief Operating Officer</span>
				</div>
			</div>
	
			<div class="flex flex-col gap-8 items-center">
				<img src={thirdPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center">Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces">Jennie F.</span>
					<span>Business Owner</span>
				</div>
			</div>
		</div>

	</div>

	<div class="flex flex-col items-center gap-5 bg-[#90D4C5]">
		<div class="flex flex-row w-full h-auto">
			<img src={milkBottles} alt="" class="w-3/12 h-auto">
			<img src={orangeSecond} alt="" class="w-3/12 h-auto">
			<img src={conesSecond} alt="" class="w-3/12 h-auto">
			<img src={sugarCubes} alt="" class="w-3/12 h-auto">
		</div>
		<div class="flex flex-col gap-4 pt-20">
			<img src={logo} alt="">
			<div class="flex flex-row gap-6">
				<span>About</span>
				<span>Services</span>
				<span>Projects</span>
			</div>
		</div>
		<div class="flex flex-row gap-4 pb-20">
			<img src={facebook} alt="" class="w-6 h-6">
			<img src={instagram} alt="" class="w-6 h-6">
			<img src={twitter} alt="" class="w-6 h-6">
			<img src={pinterest} alt="" class="w-6 h-6">
		</div>
	</div>

</section>