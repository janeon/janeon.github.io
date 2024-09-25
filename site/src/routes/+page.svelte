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
					<img src="./twitter.svg" alt="Twitter" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://scholar.google.com/citations?user=-Dab8wMAAAAJ&hl" target="_blank">
					<img src="./scholar.svg" alt="Google Scholar" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://github.com/janeon" target="_blank">
					<img src="./github.svg" alt="GitHub" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://www.linkedin.com/in/jane-hsieh/" target="_blank">
					<img src="./linkedin.svg" alt="LinkedIn" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="https://www.instagram.com/janeon32" target="_blank">
					<img src="./insta.svg" alt="Instagram" class="h-5 w-5" />
				</a>
				<span>|</span>
				<a href="http://facebook.com/jwhsieh98" target="_blank">
					<img src="./fb.svg" alt="Facebook" class="h-5 w-5" />
				</a>
			</div>
		</div>
		<div class="mt-4 flex flex-col items-start items-center">
			<!-- Added margin top for spacing -->
			<Unscramble inputText="janeon@cmu.edu" />
			<a
				href="https://se-phd.s3d.cmu.edu/People/students/index.html"
				class="mt-2 text-sm leading-loose text-blue-500 hover:underline"
			>
				PhD Student in Software Engineering
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
					I am currently a fifth year doctoral student at
					<a href="https://s3d.cs.cmu.edu/" class="text-blue-500 hover:underline">CMU S3D</a>
					advised by Professor
					<a href="https://www.haiyizhu.com/" class="text-blue-500 hover:underline">Haiyi Zhu</a>
					from the
					<a href="https://hci.cs.cmu.edu/" class="text-blue-500 hover:underline"
						>Human Computer Interaction Institute</a
					>.
				</p>
				<p class="font-titillium mt-4 leading-relaxed text-gray-700 dark:text-gray-400">
					I research ways of alleviating impacts of algorithmically managed work using
					<a
						href="https://dl.acm.org/doi/abs/10.1145/3563657.3595982"
						class="text-blue-500 hover:underline">design</a
					>,
					<a
						href="https://dl.acm.org/doi/abs/10.1145/3491102.3517546"
						class="text-blue-500 hover:underline">empirical</a
					>, and
					<a href="https://gigshare.web.app/" class="text-blue-500 hover:underline"
						>systems-building</a
					>
					methods. Specifically, I design and build systems that engage with multiple stakeholder groups,
					so as to develop policy and technology innovations that engender more equitable, empowered,
					and sustainable futures of platform-based labor.
				</p>
			</Card>

			<Card class="font-titillium mb-4 w-full max-w-2xl leading-relaxed">
				Beyond research, I also:
				<ul class="mt-2 list-inside list-disc">
					<li>
						Organize for CMU's <a
							href="https://www.cs.cmu.edu/academics/phd/application-support"
							class="text-blue-500 hover:underline"
						>
							Graduate Application Support Program
						</a>
						<ul class="ml-4 list-inside list-disc">
							<li>To help future CMU SCS PhD applicants!</li>
						</ul>
					</li>
					<li>
						Served as a TA for
						<a
							href="https://sites.google.com/andrew.cmu.edu/haii-cmu/"
							class="text-blue-500 hover:underline"
						>
							Human-AI Interaction</a
						>
					</li>
					<li>
						Receive generous support from the <a
							href="https://www.nsfgrfp.org/"
							class="text-blue-500 hover:underline"
						>
							NSF Graduate Research Fellowship</a
						>
					</li>
					<li>
						Marvel at <a
							href="https://www.instagram.com/truffle_hsieh/"
							class="text-blue-500 hover:underline">Truffle's</a
						> adorableness
					</li>
					<li>
						<a href="https://www.goodreads.com/user/show/141589623-jane-hsieh" class="text-blue-500 hover:underline">Read</a>, <a href="https://www.xiachufang.com/cook/121052741/" class="text-blue-500 hover:underline">cook</a>, <a href="https://www.reimaginedrecycling.com/" class="text-blue-500 hover:underline">recycle</a>, woodwork/3D-print, and occasionally revisit the violin
					</li>
				</ul>
			</Card>

			<Card class="mb-4 w-full max-w-2xl leading-relaxed">
				<p class="font-titillium text-gray-700 dark:text-gray-400">
					Before CMU, I graduated <a href="https://www.oberlin.edu/" class="text-blue-500 hover:underline">Oberlin College</a> with a BA in <a href="https://www.cs.oberlin.edu/">CS</a> and <a href="https://www.oberlin.edu/arts-and-sciences/departments/mathematics" class="text-blue-500 hover:underline">Math</a> (along with a <a href="https://www.oberlin.edu/cognitive-sciences" class="text-blue-500 hover:underline">Cognitive Science concentration</a>), where I was advised academically by <a href="https://www.cs.oberlin.edu/~bob/" class="text-blue-500 hover:underline">Bob Geitz</a> and <a href="http://www.dominoartwork.com/" class="text-blue-500 hover:underline">Bob Bosch</a>, and research-wise by <a href="https://cs.oberlin.edu/~ctaylor/" class="text-blue-500 hover:underline">Cynthia Tayler</a> and <a href="https://www.oberlin.edu/yumi-ijiri" class="text-blue-500 hover:underline">Yumi Ijiri</a>.
					
				</p>
				
			</Card>
			
		</div>
	</div>
</div>
