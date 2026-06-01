<script lang="ts">
	import { Avatar, Card } from 'flowbite-svelte';
	import Unscramble from '../lib/Unscramble.svelte';
</script>

<div class="container mx-auto ml-5 flex flex-col md:ml-0 md:flex-row mr-8 pr-8">
	<div class="mx-auto mb-4 flex flex-col items-start pl-4 md:mx-0 md:mb-0 md:mr-4">
		<div class="flex flex-col items-center">
			<Avatar src="./photoshoot.jpeg" size="xl" class="mx-2 rounded-full" />
			<div class="mt-2 flex items-center space-x-2">
				<a href="https://twitter.com/Jane_Hsieh32" target="_blank">
					<img src="/twitter.svg" alt="Twitter" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://scholar.google.com/citations?user=-Dab8wMAAAAJ&hl" target="_blank">
					<img src="/scholar.svg" alt="Google Scholar" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://github.com/janeon" target="_blank">
					<img src="/github.svg" alt="GitHub" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://www.linkedin.com/in/jane-hsieh/" target="_blank">
					<img src="/linkedin.svg" alt="LinkedIn" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://www.instagram.com/janeon32" target="_blank">
					<img src="/insta.svg" alt="Instagram" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="http://facebook.com/jwhsieh98" target="_blank">
					<img src="/fb.svg" alt="Facebook" class="h-5 w-5" />
				</a>
			</div>
		</div>
		<div class="mt-4 flex flex-col items-start items-center">
			<!-- Added margin top for spacing -->
			<Unscramble inputText="janeon@cmu.edu" />
			<a
				href="https://se-phd.s3d.cmu.edu/People/alumni/hsieh-jane.html"
				class="mt-2 text-sm leading-loose text-blue-500 hover:underline"
			>
				Software Engineering PhD 
			</a>
			<a
				href="https://www.cs.cmu.edu/"
				class="mt-1 text-sm leading-loose text-blue-500 hover:underline"
			>
				School of Computer Science
			</a>
		</div>
	</div>

	<div class="ml-4 flex flex-grow flex-col mr-6">
		<div class="flex flex-col items-center">
			<!-- Changed to flex-col and added items-center -->
			<Card class="mb-4 w-full max-w-2xl">
				<!-- Added margin bottom for spacing -->
				<h5 class="tracking-loose mb-2 text-2xl font-bold text-gray-900 dark:text-white">Howdy!</h5>
				<p class="font-titillium leading-relaxed text-gray-700 dark:text-gray-400">
					I am a recent Software Engineering PhD graduate from
					<a href="https://se-phd.s3d.cmu.edu/" class="text-blue-500 hover:underline">CMU S3D</a>
					advised by
					Prof. <a href="https://www.haiyizhu.com/" class="text-blue-500 hover:underline">Haiyi Zhu</a> as a part of the <a href="https://www.social-ai.org/" class="text-blue-500 hover:underline">Social AI Lab</a>. Currently, I research at the
					<a href="https://hci.cs.cmu.edu/" class="text-blue-500 hover:underline"
						>Human Computer Interaction Institute</a
					>.
				</p>
				<p class="font-titillium mt-4 leading-relaxed text-gray-700 dark:text-gray-400">
					My research focuses on understanding and reshaping how disruptive technologies such as gig platforms interact with and impact worker and user communities, so as to design and promote more <b>collective</b>, <b>safe</b> and <b>prosperous futures of work</b>.
					
					To reach this objective, I employ grounded, multi-stakeholder approaches such as 
					<a
						href="https://dl.acm.org/doi/abs/10.1145/3563657.3595982"
						class="text-blue-500 hover:underline">qualitative co-design</a
					> and
					<a href="https://gigshare.web.app/" class="text-blue-500 hover:underline"
						>systems-building</a
					> to develop technology probes that motivate transformative (pro)social behaviors, as well as
					 more scalable  
					<a
						href="https://dl.acm.org/doi/abs/10.1145/3491102.3517546"
						class="text-blue-500 hover:underline">quantitative empirical</a> methods to observe effects of interventions and naturally-occurring phenomena.

				<p class="font-titillium mt-4 leading-relaxed text-gray-700 dark:text-gray-400">
					This work has been recognized by the the <a
							href="https://janeon.github.io/grfp.pdf"
							class="text-blue-500 hover:underline"
						>
							NSF Graduate Research Fellowship</a
						> as well as best paper awards at leading HCI conferences including ACM CHI, CHIWORK and UIST. My PhD has also been generously funded by the <a href="https://www.cmu.edu/block-center/future-of-work" class="text-blue-500 hover:underline">CMU Block Center for Technology and Society.</a>
						
						Previously, I graduated <a href="https://www.oberlin.edu/" class="text-blue-500 hover:underline">Oberlin College</a> magna cum laude
						with a BA in <a href="https://www.cs.oberlin.edu/" class="text-blue-500 hover:underline">CS</a>, <a href="https://www.oberlin.edu/arts-and-sciences/departments/mathematics" class="text-blue-500 hover:underline">Math</a>, and <a href="https://www.oberlin.edu/cognitive-sciences" class="text-blue-500 hover:underline">Cognitive Science</a>, as a <a href="https://www.oberlin.edu/undergraduate-research/programs/strong" class="text-blue-500 hover:underline">STRONG</a> and <a href="https://hluce.org/programs/clare-boothe-luce/" class="text-blue-500 hover:underline">Clare Boothe Luce</a> Scholar.
				</p>
				<br />
						<b>
						I am on the job market. 
						</b>
			</Card>

			<Card class="font-titillium mb-4 w-full max-w-2xl leading-relaxed">
				Outside of research, you can find me bouncing furiously between
				<ul class="mt-2 list-inside list-disc">
					<!-- <li>
						Organize for CMU's <a
							href="https://www.cs.cmu.edu/academics/phd/application-support"
							class="text-blue-500 hover:underline"
						>
							Graduate Application Support Program
						</a>
					</li>
					<li>
						Served as a TA for
						<a
							href="https://sites.google.com/andrew.cmu.edu/haii-cmu/"
							class="text-blue-500 hover:underline"
						>
							Human-AI Interaction</a
						>
					</li> -->
					<li>
						Marveling at <a
							href="https://www.instagram.com/truffle_hsieh/"
							class="text-blue-500 hover:underline">Truffle's</a
						> adorableness 🐶
					</li>
					<li>
						<a href="https://www.xiachufang.com/cook/121052741/" class="text-blue-500 hover:underline">Cooking 🍲</a> (usually soups and/or noodles) and sometimes baking 🍰
					</li>
					<li><a href="https://www.goodreads.com/user/show/141589623-jane-hsieh" class="text-blue-500 hover:underline">Reading 📚</a>, hiking 🚶‍♀️🌲 or discovering new tea shops 🍵</li>
					<li>
						Exploring new cities with my bike helmet on local bike/scooter-share 🚴‍♀️
					</li>
					<li>
						Volunteering for causes like <a href="https://www.reimaginedrecycling.com/" class="text-blue-500 hover:underline">recycling ♻️</a>
					</li>
					<li>Playing puzzles 🧩 and <a href="https://steamcommunity.com/profiles/76561198986320571/" class="text-blue-500 hover:underline">games</a> 🎮 recreationally</li>
					<li>Woodworking 🪵, 3D-printing or occasionally revisiting the violin 🎻</li>
				</ul>
			</Card>

			<!-- <Card class="mb-4 w-full max-w-2xl leading-relaxed">
				<p class="font-titillium text-gray-700 dark:text-gray-400">
										
				</p>
				
			</Card> -->
			
		</div>
	</div>
</div>
