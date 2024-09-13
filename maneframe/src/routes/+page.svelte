<script>
	import Counter from "./Counter.svelte";
	import welcome from "$lib/images/svelte-welcome.webp";
	import welcome_fallback from "$lib/images/svelte-welcome.png";
	import { browser } from "$app/environment";

	import Typewriter from "svelte-typewriter";
</script>

<html lang="en">
	<body
		class="overflow-x-hidden w-screen h-screen bg-gradient-to-b from-black to-indigo-900 resize-none scroll-smooth"
	>
		<div class="navbar bg-gray-900 fixed top-0 w-full z-10">
			<div class="navbar-start">
				<div class="dropdown">
					<div
						tabindex="0"
						role="button"
						class="btn btn-ghost lg:hidden"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							class="h-5 w-5"
							fill="none"
							viewBox="0 0 24 24"
							stroke="currentColor"
							><path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M4 6h16M4 12h8m-8 6h16"
							/></svg
						>
					</div>
					<ul
						tabindex="0"
						class="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-base-100 rounded-box w-52"
					>
						<li><a href="/#FAQ">FAQ</a></li>
						<li><a href="/#GS">Guest Speakers</a></li>
						<li><a href="/#SCHED">Schedule</a></li>
						<li><a href="https://sjpl.bibliocommons.com/events/66df4512506577776c4af422">Apply</a></li>
					</ul>
				</div>
				<a class="btn btn-ghost text-xl text-white" href="/"
					>ManeFrame</a
				>
				<div class="w-10 rounded-full m-2">
					<img alt="ManeFrame" src="/img.png" />
				</div>
			</div>
			<div class="navbar-center hidden lg:flex">
				<ul class="menu menu-horizontal px-1">
					<li><a href="/#ABT" class="text-xl text-white">About Us</a></li>
					<li><a href="/#FAQ" class="text-xl text-white">FAQ</a></li>
					<li>
						<a href="/#GS" class="text-xl text-white"
							>Guest Speakers</a
						>
					</li>
					<li>
						<a href="/#SCHED" class="text-xl text-white">Schedule</a
						>
					</li>
					<li>
						<a href="https://sjpl.bibliocommons.com/events/66df4512506577776c4af422" class="text-xl text-white">Apply</a>
					</li>
				</ul>
			</div>
			<div class="navbar-end">
				<div class="w-10 rounded-full mr-2">
					<a href="https://discord.gg/JSRUHBAG" target="_blank">
						<img alt="DC" src="/icons8-discord-48.png" />
					</a>
				</div>
				<div class="w-10 rounded-full mr-2">
					<a
						href="https://instagram.com/maneframe2024"
						target="_blank"
					>
						<img alt="IG" src="/icons8-instagram-48.png" />
					</a>
				</div>
				<div class="w-10 rounded-full mr-10">
					<a href="mailto:maneframe24@gmail.com" target="_blank">
						<img alt="SMTP" src="/icons8-email-48.png" />
					</a>
				</div>
			</div>
		</div>
		<div class="w-screen mt-16 mb-4">
			<img
				src="/img.png"
				alt="logo"
				class="m-auto object-scale-down"
				width="300"
			/>
		</div>
		<div
			class="w-screen text-center items-center content-center justify-center mb-1"
		>
			<h1
				class="text-7xl lg:text-9xl font-bold animate-bounce-small sm:text-center text-white pt-12 mb-10 sm:m-20 sm:mt-16"
			>
				ManeFrame
			</h1>
			<Typewriter mode="loop" wordInterval="3000" class="">
				<p
					class="text-2xl sm:text-5xl font-italic, text-center, animate-pulse text-white m-10"
					id="llvm"
				>
					A Hackathon for Middle and High School Students
				</p>
				<p
					class="text-2xl sm:text-5xl font-italic, text-center, animate-pulse text-white m-10"
				>
					October 19th @ MLK Library, San Jose State University
				</p>
			</Typewriter>
		</div>
		<!-- <div class="divider text-white divider-white sm:text-4xl">
		</div> -->

		<div
			class="w-screen flex text-center content-center justify-center content-center"
		>
			<div class="text-center w-3/4 sm:w-1/2 sm:m-12">
				<a href="https://sjpl.bibliocommons.com/events/66df4512506577776c4af422" id="llvmrefernce"
					><button
						class="button bg-white text-black text-xl md:text-2xl p-4 2xl:p-10 md:m-2 rounded-xl"
						>APPLY</button
					></a
				>
			</div>
		</div>
		<div class="w-screen flex text-center content-center justify-center">
			<div class="text-center w-3/4 sm:w-1/2 sm:m-12">
				<h1
					class="text-white text-3xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 lg:mt-2 mt-8 font-bold mb-8 p-4 hover:animate-pulse"
				>
					Hey!
				</h1>
				<p
					class="text-white text-xl lg:text-2xl 2xl:text3xl text-center justify-center content-center mb-4"
				>
					Do you want to make something cool? Spend some time with
					friends? Or maybe learn something new? If so, you should
					come to the ManeFrame hackathon! Whether you're a seasoned
					programmer or just starting out, we have a place for you!
				</p>
		
			</div>
		</div>
		<div class="divider text-white divider-white sm:text-4xl"></div>
		<!---->
		<div class="divider text-white divider-white sm:text-4xl sm:mt-8"></div>
		<div class="w-screen flex text-center content-center justify-center">
			<div class="text-center w-3/4 sm:w-1/2 sm:m-12">
				<h1
					class="text-white text-3xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 lg:mt-2 mt-8 font-bold mb-8 hover:animate-pulse" id="ABT"
				>
					About Us
				</h1>
				<p
					class="text-white text-xl lg:text-2xl 2xl:text3xl text-center justify-center content-center mb-4"
				>
				ManeFrame 2024 is organized by a team of high school
				students in the Bay Area passionate about all aspects of
				computer science, from machine learning to web development
				and everything in between. With top-tier workshops and
				mentors, we aim to foster an environment of collaboration
				and hands-on learning to spark innovation in the minds of
				this young generation. With the help of San Jose Public
				Library and San Jose State University, we promise to make the most engaging and truly fun
				coding-based event we truly can! Maneframe2024 will be taking place on October 19th, 2024.
				</p>
			
			</div>
		</div>
		<div class="divider text-white divider-white sm:text-4xl"></div>
		<!---->
		<div class="divider text-white divider-white sm:text-4xl sm:mt-8"></div>
		<div class="w-screen flex text-center content-center justify-center">
			<div class="text-center w-3/4 sm:w-1/2 sm:m-8">
				<h1
					class="text-white text-2xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 lg:mt-2 mt-8 font-bold hover:animate-pulse"
					id="FAQ"
				>
					Frequently Asked Questions
				</h1>
			</div>
		</div>
		<div class="w-screen lg:flex text-center content-center justify-center">
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-white text-3xl lg:text-2xl xl:text-4xl lg:ml-8 lg:mr-8 font-bold mb-8 mt-8 hover:animate-pulse"
				>
					What is a Hackathon?
				</h1>
				<p
					class="text-white text-md lg:text-xl text-center justify-center content-center mb-4"
				>
					A Hackathon is an event where you code a project for a
					certain amount of time and then get it judged. It is meant
					to be a fun event where you can create anything you want
					with freedom, and where you can explore the amazing world of
					computer science.
				</p>
			</div>
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-white text-3xl lg:text-2xl xl:text-4xl lg:ml-8 lg:mr-8 font-bold mb-8 mt-8 hover:animate-pulse"
				>
					What do I make?
				</h1>
				<p
					class="text-white text-md lg:text-xl text-center justify-center content-center mb-4"
				>
					You can make whatever you want! From a simple calculator app
					to an online chat portal, feel free to make or submit
					anything. We encourage exploring and trying out new things!
				</p>
			</div>
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-white text-3xl lg:text-2xl xl:text-4xl lg:ml-8 lg:mr-8 font-bold mb-8 mt-8 hover:animate-pulse"
				>
					Does it cost money?
				</h1>
				<p
					class="text-white text-md lg:text-xl text-center justify-center content-center mb-4"
				>
					Nope! Maneframe is absolutely free! We encourage anyone in
					middle or high school to attend.
				</p>
			</div>
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-white text-3xl lg:text-2xl xl:text-4xl lg:ml-8 lg:mr-8 font-bold mb-8 mt-8 hover:animate-pulse"
				>
					Do I need a team?
				</h1>
				<p
					class="text-white text-md lg:text-xl text-center justify-center content-center mb-4"
				>
					A team is not necessary, but working in a team is a great
					way to collaborate with like-minded peers! We will have a
					Team Mixer, or an event to allocate teams, if you are unsure
					who to team up with.
				</p>
			</div>
		</div>
		<p class="text-xl text-white mt-10 text-center text-bold">Also, please bring your own device!</p>
		<div class="divider text-white divider-white sm:text-4xl sm:mt-8"></div>
		<!---->
		<div class="divider text-white divider-white sm:text-4xl sm:mt-8"></div>
		<div class="w-screen flex text-center content-center justify-center">
			<div class="text-center w-3/4 sm:w-1/2 sm:m-8">
				<h1
					class="text-white text-2xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 lg:mt-2 mt-8 font-bold hover:animate-pulse"
					id="GS"
				>
					Guest Speakers
				</h1>
			</div>
		</div>
		<div class="w-screen lg:flex text-center content-center justify-center">
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-2xl mb-10 text-white decoration-dashed"
				>
					Viraj Kadakia
				</h1>
				<img
					src="viraj.jpeg"
					alt="Viraj Kadakia"
					width="200"
					class="m-auto"
				/>
				<h3 class="text-md mt-10 mb-10 text-white">
					Viraj Kadakia is a skilled software engineer specializing in
					backend and web development at CloudTrucks, with previous
					experience at Amazon and internships at StubHub and
					LendingClub. He holds a Bachelor's degree in Computer
					Science from UC Berkeley and has developed notable projects
					like the Receipt Allocator, an expense management tool, and
					HalfWay, a meeting location optimizer.
				</h3>
			</div>
			<div
				class="text-center lg:w-1/4 m-10 p-4 border-white rounded-md border-2"
			>
				<h1
					class="text-2xl mb-10 text-white decoration-dashed"
				>
					Sagar Joshi
				</h1>
				<img
					src="sagar.jpeg"
					alt="Sagar Joshi"
					width="200"
					class="m-auto"
				/>
				<h3 class="text-md mb-10 mt-10 text-white">
					Sagar Suhas Joshi is a roboticist specializing in motion
					planning at Aurora Innovation. He earned his PhD in robotics
					from Georgia Tech in 2022, where he developed intelligent
					exploration algorithms for efficient motion planning and
					learning. With a background from IIT-Madras, Sagar's work
					intersects A.I., machine learning, and optimal-control
					theory.
				</h3>
			</div>
		</div>
		<div class="divider text-white divider-white sm:text-4xl sm:mt-8"></div>
		<!---->
		<div
			class="divider text-white divider-white sm:text-4xl sm:mt-8 mb-2"
		></div>

		<div
			class="w-screen h-1/2 text-center content-center justify-center content-center"
		>
			<div class="text-center">
				<h1
					class="text-white text-2xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 mt-2 font-bold mb-8 hover:animate-pulse"
					id="SCHED"
				>
					Schedule
				</h1>

				<div class="overflow-x-auto w-screen flex justify-center mb-20">
					<table class="table bg-black bg-opacity-40 w-1/2">
						<!-- head -->
						<thead>
							<tr>
								<th class="text-white">Time</th>
								<th class="text-white">Event</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td class="text-white">9:00 - 9:15 A.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Doors Open
									</h1>
									<h1 class="text-white text-xs mt-2">
										Welcome participants and get ready for
										an exciting day of hacking.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">9:15 - 9:30 A.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Hacking Begins!!
									</h1>
									<h1 class="text-white text-xs mt-2">
										Kick-off the hackathon with an official
										start to the coding session.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">9:30 - 10:00 A.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Team Mixer
									</h1>
									<h1 class="text-white text-xs mt-2">
										A fun session to form teams, network,
										and brainstorm ideas.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">10:00 A.M. - 12:00 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										First Coding Session
									</h1>
									<h1 class="text-white text-xs mt-2">
										Dive into your projects and start
										coding.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">12:00 - 1:00 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Lunch
									</h1>
									<h1 class="text-white text-xs mt-2">
										Take a break and enjoy a meal to
										recharge for the afternoon.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">1:00 - 2:00 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Second Coding Session
									</h1>
									<h1 class="text-white text-xs mt-2">
										Continue working on your projects with
										your team.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">2:00 - 2:30 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Guest Speakers
									</h1>
									<h1 class="text-white text-xs mt-2">
										Hear from industry leaders and
										innovators during our guest speaker
										session.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">2:30 - 3:45 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Third Coding Session
									</h1>
									<h1 class="text-white text-xs mt-2">
										Make the final touches to your projects
										before the deadline.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">3:45 - 4:15 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Demos
									</h1>
									<h1 class="text-white text-xs mt-2">
										Showcase your projects and see what
										others have created.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">4:15 - 4:45 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Judging/Voting
									</h1>
									<h1 class="text-white text-xs mt-2">
										Judges review the projects and
										participants vote for their favorites.
									</h1>
								</td>
							</tr>

							<tr>
								<td class="text-white">4:45 - 5:00 P.M.</td>
								<td class="text-white">
									<h1 class="text-white text-md font-bold">
										Winner and Award Ceremony
									</h1>
									<h1 class="text-white text-xs mt-2">
										Announce the winners and celebrate the
										achievements of all participants.
									</h1>
								</td>
							</tr>
						</tbody>
					</table>
				</div>
				<!-- <table class="table-auto border-2 border-accent border-separate">
						<tr>
							<th class="border border-accent">Time</th>
							<th class="border border-accent">Event</th>
						</tr>
						<tr>
							<td>9:30 - 10:00 A.M.</td>
							<td>Doors Open!</td>
						</tr>
						<tr>
							<td>10:00 - 10:15 A.M.</td>
							<td>Hacking Begins!!</td>
						</tr>
						<tr>
							<td>9:30 A.M.</td>
							<td>Breakfast</td>
						</tr>
						<tr>
							<td>10:15 - 10:30 A.M.</td>
							<td>Team Mixer</td>
						</tr>
						<tr>
							<td>10:30 - 11:30 A.M.</td>
							<td>Workshops</td>
						</tr>
						<tr>
							<td>12:00 - 12:30 P.M.</td>
							<td>Lunch</td>
						</tr>
						<tr>
							<td>1:30 - 2:30 P.M.</td>
							<td>Panelists</td>
						</tr>
						<tr>
							<td>3:30 P.M.</td>
							<td>Project Deadline</td>
						</tr>
						<tr>
							<td>3:30 - 4:30 P.M.</td>
							<td>Demos</td>
						</tr>
						<tr>
							<td>4:30 - 4:45 P.M.</td>
							<td>Judging/Voting</td>
						</tr>
						<tr>
							<td>4:45 - 5:00 P.M.</td>
							<td>Winner and Award Ceremony</td>
						</tr>
					</table> -->
			</div>
			<div
				class="divider text-white divider-white sm:text-4xl sm:mt-8"
			></div>
			<!---->
			<div
				class="divider text-white divider-white sm:text-4xl sm:mt-8"
			></div>
			<h1
				class="text-white text-2xl lg:text-3xl xl:text-5xl xl:mt-16 lg:ml-16 lg:mr-16 mt-2 font-bold mb-8 hover:animate-pulse"
			>
				Sponsors
			</h1>
			<div class="flex content-center justify-center mb-20">
				<div class="text-center sm:w-1/4 m-10">
					<img src="sjsu.png" alt="SJSU" width="500" class="m-auto" />
					<img
						src="sjpl2.png"
						alt="SJPL"
						width="500"
						class="m-auto"
					/>
				</div>
			</div>
		</div>

		<br />
	</body>
</html>
