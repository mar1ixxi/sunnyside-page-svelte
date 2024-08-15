<script>
	import logo from '$lib/images/logo.svg';
	import down_arrow from '$lib/images/icon-arrow-down.svg';
	import hamburger from '$lib/images/icon-hamburger.svg';
	import triangle from '$lib/images/triangle-arrow.svg';

	import main_bg from '$lib/images/desktop/image-header.jpg';
	import mobile_bg from '$lib/images/mobile/image-header.jpg';

	// For desktop
	import egg_bg from '$lib/images/desktop/image-transform.jpg';
	import cup from '$lib/images/desktop/image-stand-out.jpg';
	import cherry from '$lib/images/desktop/image-graphic-design.jpg';
	import orange from '$lib/images/desktop/image-photography.jpg';
	
	// For mobiles
	import mobile_egg_bg from '$lib/images/mobile/image-transform.jpg';
	import mobile_cup from '$lib/images/mobile/image-stand-out.jpg';
	import mobile_cherry from '$lib/images/mobile/image-graphic-design.jpg';
	import mobile_orange from '$lib/images/mobile/image-photography.jpg';

	import firstPerson from '$lib/images/image-emily.jpg';
	import secondPerson from '$lib/images/image-jennie.jpg';
	import thirdPerson from '$lib/images/image-thomas.jpg';

	// For desktop
	import milkBottles from '$lib/images/desktop/image-gallery-milkbottles.jpg'
	import orangeSecond from '$lib/images/desktop/image-gallery-orange.jpg'
	import conesSecond from '$lib/images/desktop/image-gallery-cone.jpg'
	import sugarCubes from '$lib/images/desktop/image-gallery-sugarcubes.jpg'
	
	// For mobiles
	import mobile_milkBottles from '$lib/images/mobile/image-gallery-milkbottles.jpg'
	import mobile_orangeSecond from '$lib/images/mobile/image-gallery-orange.jpg'
	import mobile_conesSecond from '$lib/images/mobile/image-gallery-cone.jpg'
	import mobile_sugarCubes from '$lib/images/mobile/image-gallery-sugar-cubes.jpg'

	// Logo are imported here
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

	<div class="w-full md:min-h-screen min-h-auto h-full flex flex-col gap-20 items-center justify-center relative">

		<nav class="absolute flex flex-row justify-between top-4 w-full h-auto md:px-12 px-8 py-2">
			<img src={logo} alt="" class="w-auto md:h-8 h-5">

			<div class="md:flex hidden font-barlow font-semibold text-white text-base gap-12 items-center justify-center">
				<span class="cursor-pointer">About</span>
				<span class="cursor-pointer">Services</span>
				<span class="cursor-pointer">Projects</span>
				<span class="py-3 px-6 rounded-full transition-all bg-white hover:bg-[#5AC8FF] text-black hover:text-white font-fraunces uppercase cursor-pointer">Contact</span>
			</div>

			<div class="md:hidden flex hamburger">
				<img src={hamburger} alt="" class="h-4 transition-all">

				<img src={triangle} alt="" class="absolute right-[8.8%] top-10 triangle">
				<div class='tab-section absolute top-16 left-[8%] z-10 py-6 flex flex-col font-barlow font-medium text-[#A7ABAE] text-lg gap-6 items-center justify-center bg-white w-10/12 h-auto'>
					<span class="cursor-pointer">About</span>
					<span class="cursor-pointer">Services</span>
					<span class="cursor-pointer">Projects</span>
					<span class="py-3 px-6 rounded-full transition-all bg-[#FAD400] text-black hover:text-white font-fraunces uppercase cursor-pointer">Contact</span>
				</div>

			</div>

		</nav>

		<div class="absolute flex flex-col gap-20 items-center text-center top-[30%]">
			<h3 class="md:text-6xl text-4xl text-white font-black tracking-wider font-fraunces uppercase">We are creatives</h3>
			<img src={down_arrow} alt="" class="w-8 h-auto" />
		</div>

		<img src={main_bg} alt="" class="md:flex hidden w-full h-full object-cover">
		<img src={mobile_bg} alt="" class="md:hidden flex w-full h-full object-cover">

	</div>

	<div class="w-full h-auto flex flex-col font-fraunces">
		<div class="flex md:flex-row flex-col-reverse w-full h-auto">
			
			<div class="md:w-1/2 w-full h-auto md:p-40 p-5 md:py-40 py-20 flex flex-col md:items-start items-center gap-6 md:text-left text-center">
				<div class="text-4xl font-bold text-black">Transform your brand</div>
				<div class='font-barlow text-lg font-medium text-[#5A636C]'>
					We are a full-service creative agency specializing in helping brands grow fast. 
					Engage your clients through compelling visuals that do most of the marketing for you.
				</div>
				<button class="red-btn transition-all relative px-2 flex justify-center">
					<div class="uppercase relative z-10 text-black">Learn more</div>
					<span class='bg-[#FCEFB9] absolute top-3 w-full h-2.5 rounded z-0 yellowLine' />
				</button>
			</div>

			<img src={egg_bg} alt="" class="md:w-1/2 w-full md:flex hidden h-full" />
			<img src={mobile_egg_bg} alt="" class="md:w-1/2 w-full md:hidden flex h-full" />

		</div>
	</div>

	<div class="w-full h-auto flex flex-col font-fraunces">
		<div class="flex md:flex-row flex-col w-full h-auto">

			<img src={cup} alt="" class="md:w-1/2 w-full md:flex hidden h-full" />
			<img src={mobile_cup} alt="" class="md:w-1/2 w-full md:hidden flex h-full" />

			<div class="md:w-1/2 w-full h-auto md:p-40 p-5 md:py-40 py-20 flex flex-col md:items-start items-center gap-6 md:text-left text-center">
				<div class="text-4xl font-bold text-black">Stand out to the right audience</div>
				<div class="font-barlow text-lg font-medium text-[#5A636C]">
					Using a collaborative formula of designers, researchers, photographers, videographers, and copywriters, we’ll build and extend your brand in digital places.
				</div>
				<button class="red-btn transition-all relative px-2 flex justify-center">
					<div class="uppercase relative z-10 text-black">Learn more</div>
					<span class=' md:flex hidden absolute top-3 w-full h-2.5 rounded z-0 bg-[#FBD8CF] redLine' />
				</button>
			</div>
		</div>
	</div>

	<div class="w-full h-auto flex flex-col">
		<div class="flex md:flex-row flex-col w-full h-auto">
			<div class="md:w-1/2 w-full h-full bg-cherry relative flex items-center justify-center">

				<img src={cherry} alt="" class="w-full h-full md:flex hidden" />
				<img src={mobile_cherry} alt="" class="w-full h-full md:hidden flex" />

				<div class='absolute bottom-10 flex flex-col items-center justify-center gap-4 md:w-1/2 w-11/12 text-[#25564B]'>
					<span class="text-4xl font-bold font-fraunces">Graphic design</span>
					<span class="font-barlow text-lg font-medium text-center">Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention.</span>
				</div>
			</div>
			<div class="md:w-1/2 w-full h-full bg-orange relative flex items-center justify-center">

				<img src={orange} alt="" class="w-full h-full md:flex hidden" />
				<img src={mobile_orange} alt="" class="w-full h-full md:hidden flex" />

				<div class='absolute bottom-10 flex flex-col items-center justify-center gap-4 md:w-1/2 w-11/12 text-[#19536B]'>
					<span class="text-4xl font-bold font-fraunces">Photography</span>
					<span class="font-barlow text-lg font-medium text-center">Increase your credibility by getting the most stunning, high-quality photos that improve your business image.</span>
				</div>
			</div>
		</div>
	</div>

	<div class="flex flex-col md:w-9/12 w-11/12 h-auto md:py-40 py-20 gap-20 items-center justify-center">
		<h3 class="text-2xl font-semibold font-fraunces uppercase text-[#A7ABAE]">Client testimonials</h3>

		<div class="flex md:flex-row flex-col gap-10">
			<div class="flex flex-col gap-8 items-center">
				<img src={firstPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center text-base font-barlow text-[#5A636C]">We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces font-bold">Emily R.</span>
					<span class="text-[#A7ABAE] font-barlow">Marketing Director</span>
				</div>
			</div>
	
			<div class="flex flex-col gap-8 items-center">
				<img src={secondPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center text-base font-barlow text-[#5A636C]">Sunnyside’s enthusiasm coupled with their keen interest in our brand’s success made it a satisfying and enjoyable experience.</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces font-bold">Thomas S.</span>
					<span class="text-[#A7ABAE] font-barlow">Chief Operating Officer</span>
				</div>
			</div>
	
			<div class="flex flex-col gap-8 items-center">
				<img src={thirdPerson} alt="" class="w-16 h-16 rounded-full">
				<div class="text-center text-base font-barlow text-[#5A636C]">Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!</div>
				<div class="flex flex-col gap-1 text-center">
					<span class="font-fraunces font-bold">Jennie F.</span>
					<span class="text-[#A7ABAE] font-barlow">Business Owner</span>
				</div>
			</div>
		</div>

	</div>

	<div class="flex flex-col items-center gap-8 bg-[#90D4C5]">
		<div class="md:flex hidden flex-row flex-wrap w-full h-auto">
			<img src={milkBottles} alt="" class="md:w-3/12 w-6/12 h-auto">
			<img src={orangeSecond} alt="" class="md:w-3/12 w-6/12 h-auto">
			<img src={conesSecond} alt="" class="md:w-3/12 w-6/12 h-auto">
			<img src={sugarCubes} alt="" class="md:w-3/12 w-6/12 h-auto">
		</div>

		<div class="md:hidden flex flex-row flex-wrap w-full h-auto">
			<img src={mobile_milkBottles} alt="" class="w-1/2 h-auto">
			<img src={mobile_orangeSecond} alt="" class="w-1/2 h-auto">
			<img src={mobile_conesSecond} alt="" class="w-1/2 h-auto">
			<img src={mobile_sugarCubes} alt="" class="w-1/2 h-auto">
		</div>

		<div class="flex flex-col items-center justify-center gap-8 pt-16">
			<img src={logo} alt="" class="md:w-52 w-40">
			<div class="flex flex-row gap-10 font-medium text-lg font-barlow">
				<span class=" transition-all text-[#458C7E] hover:text-white cursor-pointer">About</span>
				<span class=" transition-all text-[#458C7E] hover:text-white cursor-pointer">Services</span>
				<span class=" transition-all text-[#458C7E] hover:text-white cursor-pointer">Projects</span>
			</div>
		</div>
		<div class="flex flex-row gap-6 pt-10 pb-20">
			<img src={facebook} alt="" class="w-5 h-5 cursor-pointer">
			<img src={instagram} alt="" class="w-5 h-5 cursor-pointer">
			<img src={twitter} alt="" class="w-5 h-5 cursor-pointer">
			<img src={pinterest} alt="" class="w-5 h-5 cursor-pointer">
		</div>
	</div>

</section>