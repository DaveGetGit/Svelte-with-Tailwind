<script>
	import Step from './Step.svelte';

	let steps = [
		{
			name: 'Ethiopian Airlines Cargo Website',
			icon: 'fa-solid fa-plane',
			description:
				'Developed the Ethiopian Airlines Cargo website using ASP.NET Core and integrated REST APIs for streamlined cargo management and tracking.'
		},
		{
			name: 'Ethiopian Passport Services',
			icon: 'fa-solid fa-passport',
			description:
				'Created the Ethiopian Passport Services platform with ASP.NET technology stack, ensuring secure and efficient passport application and renewal processes.'
		},
		{
			name: 'Ethiopian Airlines Group’s Performance Management System',
			icon: 'fa-solid fa-chart-bar',
			description:
				'Engineered the Ethiopian Airlines Group’s Performance Management System, leveraging Microservices architecture and Windows Applications for comprehensive employee performance tracking and improvement.'
		},
		{
			name: 'Cargo Invoice Generator',
			icon: 'fa-solid fa-file-invoice-dollar',
			description:
				'Developed the Cargo Invoice Generator using ASP.NET Core and Azure, automating the invoice generation process for Ethiopian Airlines cargo services.'
		},
		{
			name: 'Ethiopian Airlines Corporate Website',
			icon: 'fa-solid fa-globe',
			description:
				'Contributed to the Ethiopian Airlines Corporate Website, utilizing ASP.NET and MVC framework to enhance the online presence and accessibility of the airline.'
		},
		{
			name: 'Ethiopian Airlines Group’s Performance Management System (ETGPMS)',
			icon: 'fa-solid fa-chart-line',
			description:
				'Collaborated on the development of the Ethiopian Airlines Group’s Performance Management System (ETGPMS), utilizing ASP.NET Core and Entity Framework to optimize employee performance tracking and analysis.'
		}
	];

	let benefits = [
		{
			name: 'Fast',
			description:
				'Fast load times and lag-free interactions are my highest priority. Ensuring that applications load quickly and respond instantly enhances user satisfaction and retention. By optimizing code, reducing resource usage, and leveraging efficient algorithms, I strive to deliver seamless user experiences. Additionally, I implement best practices in performance monitoring and tuning to continuously improve and maintain high performance standards.'
		},
		{
			name: 'Responsive',
			description:
				'My layouts will work on any device, big or small. By employing responsive design principles, I ensure that applications adapt seamlessly to different screen sizes and resolutions. This involves using flexible grids, scalable images, and media queries to provide a consistent user experience across desktops, tablets, and smartphones. Additionally, I rigorously test layouts on various devices to guarantee compatibility and usability.'
		},
		{
			name: 'Intuitive',
			description:
				'I have a strong preference for easy-to-use, intuitive UX/UI. Designing with the user in mind, I prioritize creating interfaces that are straightforward and engaging. By conducting user research and usability testing, I ensure that every element is accessible and simple to navigate. Additionally, I adhere to established design principles and guidelines to provide a cohesive and pleasant user experience.'
		},
		{
			name: 'Dynamic',
			description:
				"Websites don't have to be static; I love making pages come to life. Utilizing dynamic elements such as animations, transitions, and interactive features, I enhance user engagement and captivate audiences. By incorporating modern web technologies like JavaScript frameworks and CSS animations, I bring creativity and vitality to each web page. Additionally, I stay updated on emerging trends and techniques to continually push the boundaries of web design and development."
		}
	];
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="introPage" class="grid grid-cols lg:grid-cols-2 gap-10 py-8 sm:py-14">
		<div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				Hi, I'm <span class="poppins text-violet-400"> Dawit </span> Mulie <br />
				<span class="poppins text-violet-400">Software</span> Engineer
			</h2>
			<p class="text=base sm:text=lg md:text-xl">
				My <span class=" text-violet-400">favorite tech</span> includes JavaScript, React, Node.js, and
			</p>

			<a
				href="#"
				target="_blank"
				class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
				><div
					class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
				/>
				<h4 class="relative z-9">Get in touch &rarr;</h4>
			</a>
		</div>

		<div class="relative shadow-2xl grid place-items-center">
			<img
				src={'images/profileImg.png'}
				alt="profile of Dawit Mulie"
				class="object-contain md:object-scale-down z-[2] max-h-[70vh]"
			/>
		</div>
	</section>

	<section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
		<div class="flex flex-col gap-2 text-center">
			<h6 class="text-large sm:text-xl md:text-2xl">Here are a few of my creative endeavors</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				Curious to <span class="poppins text-violet-400">see</span> my
				<span class="poppins text-violet-400">work</span>?
			</h3>
		</div>
		<a
			href="#"
			target="_blank"
			class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4
                sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
		>
			<i class="fa-regular fa-circle-play"></i>
			<p>Watch the video</p>
		</a>
		<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
			<Step step={steps[0]}>
				<p>
					Developed the Ethiopian Airlines Cargo website using <strong class="text-violet-400"
						>ASP.NET Core</strong
					>
					and integrated <strong class="text-violet-400">REST APIs</strong> for streamlined cargo management
					and tracking.
				</p>
			</Step>
			<Step step={steps[1]}>
				<p>
					Created the Ethiopian Passport Services platform with <strong class="text-violet-400"
						>ASP.NET</strong
					> technology stack, ensuring secure and efficient passport application and renewal processes.
				</p>
			</Step>
			<Step step={steps[2]}>
				<p>
					Engineered the Ethiopian Airlines Group’s Performance Management System, leveraging <strong
						class="text-violet-400">Microservices</strong
					>
					architecture and <strong class="text-violet-400">Windows Applications</strong> for comprehensive
					employee performance tracking and improvement.
				</p>
			</Step>
			<Step step={steps[3]}>
				<p>
					Developed the Cargo Invoice Generator using <strong class="text-violet-400"
						>ASP.NET Core</strong
					>
					and <strong class="text-violet-400">Azure</strong>, automating the invoice generation
					process for Ethiopian Airlines cargo services.
				</p>
			</Step>
			<Step step={steps[4]}>
				<p>
					Contributed to the Ethiopian Airlines Corporate Website, utilizing <strong
						class="text-violet-400">ASP.NET</strong
					>
					and <strong class="text-violet-400">MVC</strong> framework to enhance the online presence and
					accessibility of the airline.
				</p>
			</Step>
			<Step step={steps[5]}>
				<p>
					Collaborated on the development of the Ethiopian Airlines Group’s Performance Management
					System (ETGPMS), utilizing <strong class="text-violet-400">ASP.NET Core</strong> and
					<strong class="text-violet-400">Entity Framework</strong> to optimize employee performance
					tracking and analysis.
				</p>
			</Step>
		</div>
	</section>

	<section
		id="about"
		class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
	>
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700
            after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4 sm:py-6 md:py-8"
		>
			<h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
			<h3 class="font-semibold text-3xl sm:text4xl md:text-5xl">
				A bit <span class="poppins text-violet-400">about</span> me.
			</h3>
		</div>
		<p class="mx-auto poppins font-semibold text-lg sm-text-xl md:text2xl">I am ...</p>
		<div class="flex flex-col gap-20 w-full mx-auto max-width-[800px]">
			{#each benefits as benefit, index}
				<div class="flex gap-6 sm:gap-8">
					<p class="poppins text-4xl sm:text-5xl md:text-6xl fontsemibold text-slate-500">
						0{index + 1}
					</p>
					<div class="flex flex-col gap-6 sm:gap-8">
						<h3 class="text-2xl sm:text-3xl md:text-5xl">
							{benefit.name}
						</h3>
						<p>{benefit.description}</p>
					</div>
				</div>
			{/each}
		</div>
		<h5 class="text-2xl sm:3xl font-semibold text-center poppins">
			The <span class="text-violet-400">Complete </span> Package
		</h5>
		<div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] w-full mx-auto">
			<table class="bg-white text-slate-700 rounded text-center">
				<thead class="border-b border-solid border-slate-200">
					<tr class="">
						<th />
						<th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
						<th class="whitespace-nowrap p-2 px-4 bg-violet-700 text-white">Me</th>
					</tr>
				</thead>
				<tbody>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold tet-sm"
							>Dedication</td
						>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
					</tr>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold tet-sm"
							>Critical Thought</td
						>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
					</tr>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold tet-sm"
							>Interpersonal Skills</td
						>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
					</tr>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold tet-sm"
							>Programming Ability</td
						>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-xmark text-slate-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
						<td class=""><i class="fa-solid fa-check text-green-500"></i></td>
					</tr>
				</tbody>
			</table>
		</div>

		<div class="mx-auto -mt-12 italic sm:hidden opacity-50">
			<p>Scroll to see more &rarr;</p>
		</div>

		<p class="mx-auto">So why not invest?</p>
	</section>
</main>
