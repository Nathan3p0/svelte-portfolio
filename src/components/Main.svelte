<script>
	import Step from './Step.svelte';

	let steps = [
		{
			name: 'SocietyWeb',
			icon: 'fa-solid fa-people-group',
			href: 'https://github.com/Nathan3p0/societyweb-client'
		},
		{
			name: 'One Love Rewards',
			icon: 'fa-solid fa-coins',
			href: 'https://github.com/Nathan3p0/one-love-rewards-client/'
		},
		{
			name: 'Slanted Headlines',
			icon: 'fa-solid fa-newspaper',
			href: 'https://github.com/Nathan3p0/slanted-headlines'
		}
	];

	let benefits = [
		{
			name: 'Full-Stack Developer Extraordinaire',
			description:
				'I excel in crafting both the front-end and back-end of web applications. With a strong background in JavaScript (React, Node.js, Express, Angular) and database expertise (MongoDB, PostgreSQL, MySQL), I create seamless, user-friendly, and efficient web solutions.'
		},
		{
			name: 'Client-Centric Communicator',
			description:
				'Effective communication is at the core of my professional approach. I leverage my background in customer service to build strong client relationships and consistently deliver projects on time. I ensure clients are informed at every project stage, fostering trust and collaboration.'
		},
		{
			name: 'Agile Problem Solver',
			description:
				"As an Agile problem solver, I'm skilled at collaborating with cross-functional teams and utilizing tools like Jira for project tracking. I thrive in Agile environments, participating in daily stand-up meetings, and maintaining momentum through weekly sprint cycles."
		},
		{
			name: 'Continuous Learning Advocate',
			description:
				'I am deeply committed to ongoing learning and personal growth, continuously enhancing my skills and staying up-to-date with the latest technologies and best practices. My dedication to learning ensures I can contribute effectively to any project or team.'
		},
		{
			name: 'Tech Stack Maestro',
			description:
				'I boast expertise in a wide range of technologies, including AWS (EC2, RDS, S3, CLI, VPC), Java (Spring, JSP, Maven, Selenium), HTML/CSS, CI/CD (Git, Jenkins, Docker, Kubernetes), and RESTful APIs and SOAP web services. This extensive tech stack proficiency equips me to handle diverse project requirements.'
		},
		{
			name: 'Educator and Mentor',
			description:
				"As a coding instructor, I've honed my ability to teach and mentor others in web development. I conduct engaging workshops, provide constructive feedback, and offer one-on-one mentoring to students, contributing to their growth and understanding."
		},
		{
			name: 'Adaptable Cybersecurity Enthusiast',
			description:
				"My ongoing pursuit of a Cybersecurity AAS degree reflects my commitment to a broader technology landscape. I've gained hands-on experience in designing secure systems, conducting vulnerability assessments, and implementing defense technologies, making me a well-rounded technologist."
		}
	];
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
		<div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				Hi! I'm <span class="poppins text-teal-400">Nate</span> Szelag <br />Full Stack
				<span class="poppins text-teal-400">Developer</span>
			</h2>
			<p class="text-base sm:text-lg md:text-xl">
				My <span class="text-teal-400">favorite tech</span> includes Java, Spring, Javascript, Angular, React, Express, Node, MongoDB,
				AWS, Docker, and REST APIs.
			</p>
			<a
				href="https://www.linkedin.com/in/nathan-szelag"
				target="_blank"
				class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
			>
				<div class="absolute top-0 right-full w-full h-full bg-teal-400 opacity-20 group-hover:translate-x-full z-0 duration-200" />
				<h4 class="relative z-9">Get in touch &rarr;</h4>
			</a>
		</div>
		<div class="relative shadow-2xl grid place-items-center">
			<img
				src={'images/profile.png'}
				alt="Emoji of Nate Szelag in a coffee pot holding a cup of coffee"
				class="object-cover z-[2] max-h-[70vh]"
			/>
		</div>
	</section>
	<section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
		<div class="flex flex-col gap-2 text-center">
			<h6 class="text-lg sm:text-xl md:text-2xl">A few of my creative endeavors.</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				Curious to <span class="poppins text-teal-400">see</span> my work?
			</h3>
		</div>
		<a
			href="https://www.youtube.com"
			target="_blank"
			class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-teal-700 duration-200"
		>
			<i class="fa-brands fa-github-alt" />
			<p>GitHub</p>
		</a>
		<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
			<Step step={steps[0]}
				><p>
					SocietyWeb is a Team Management app designed for groups like Girl Scouts or Sports Teams. It's built on a technology
					stack that includes <strong class="text-teal-400">React, Node.js + Express.js, & PostgreSQL</strong>. It also
					facilitates team communication by integrating
					<strong class="text-teal-400">Twilio SMS</strong> and <strong class="text-teal-400">SendGrid APIs</strong>. The
					development process followed a <strong class="text-teal-400">test-driven</strong> approach, with thorough testing
					conducted using
					<strong class="text-teal-400">Mocha, Chai, and Jest</strong>.
				</p></Step
			>
			<Step step={steps[1]}
				><p>
					One Love Rewards is an open-source restaurant rewards platform developed using a technology stack that includes <strong
						class="text-teal-400">React, Node.js with Express.js</strong
					>
					for building the <strong class="text-teal-400">RESTful API</strong>, and
					<strong class="text-teal-400">PostgreSQL</strong>
					for data storage. This project offered valuable insights and experience in developing a
					<strong class="text-teal-400">RESTful API</strong>. I employed
					<strong class="text-teal-400">agile methodologies</strong>, which included organizing tasks into sprints and managing
					them through a Trello board for effective <strong class="text-teal-400">project management</strong>.
				</p></Step
			>
			<Step step={steps[2]}
				><p>
					Slanted Headlines is a sentiment analysis app that utilizes headlines and content obtained from the <strong
						class="text-teal-400">News API</strong
					>. It leverages <strong class="text-teal-400">Microsoft's Sentiment Analysis API</strong> to calculate the average
					sentiment score for each news source. Please note that the API subscription is currently expired, rendering the search
					feature temporarily inactive. This project was developed using
					<strong class="text-teal-400">HTML, CSS, JavaScript, and jQuery</strong>.
				</p></Step
			>
		</div>
	</section>
	<section id="about" class="py-20 pt-10 lg:pt-16 lg-py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
		<div
			class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-teal-700
        after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-teal-700 py-4"
		>
			<h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">A bit <span class="poppins text-teal-400">about</span> me.</h3>
		</div>
		<p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am . . .</p>
		<div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
			{#each benefits as benefit, index}
				<div class="flex gap-6 sm:gap-8">
					<p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
						0{index + 1}
					</p>
					<div class="flex flex-col gap-6 sm:gap-8">
						<h3 class="text-2xl sm:text-3xl md:text-5xl">{benefit.name}</h3>
						<p>{benefit.description}</p>
					</div>
				</div>
			{/each}
		</div>
		<h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
			The <span class="text-teal-400 poppins">Complete</span> Package
		</h5>
		<div class="flex flex-col overflow-x-auto gap-10 max-w-[800px] mx-auto w-full">
			<table class="bg-white text-slate-700 rounded text-center">
				<thead class="border-b border-solid border-slate-200">
					<tr>
						<th />
						<th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
						<th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
						<th class="whitespace-nowrap bg-teal-700 text-white p-4 px-8">Me</th>
					</tr>
				</thead>
				<tbody>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Dedication</td
						>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-teal-500" /></td>
					</tr>
					<tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
							>Critical Thinking</td
						>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-teal-500" /></td>
					</tr><tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
							>Interpersonal Skills</td
						>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-teal-500" /></td>
					</tr><tr class="border-b border-solid border-slate-200">
						<td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
							>Coding Proficiency</td
						>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-slate-500" /></td>
						<td><i class="fa-solid fa-xmark text-slate-500" /></td>
						<td><i class="fa-solid fa-check text-teal-500" /></td>
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
