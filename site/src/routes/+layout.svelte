<script lang="ts">
	import { page } from '$app/stores';
	import { Navbar, NavBrand, NavUl, NavLi } from 'flowbite-svelte';
	import '../app.css';
	import { base } from '$app/paths';

	$: activeUrl = $page.url.pathname;
	let activeClass =
		'text-white bg-yellow-400 md:bg-transparent md:text-yellow-400 md:dark:text-white md:dark:bg-transparent';
	let nonActiveClass =
		'text-gray-700 hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-yellow-500 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent';
</script>
<div class="mx-auto max-w-screen-lg">
	<Navbar class="sticky top-0 z-50 bg-white">
	  <NavBrand href="/" class="ml-5 md:ml-0"> <!-- Adjust margin -->
		<span class="self-center whitespace-nowrap text-2xl font-semibold dark:text-white">
		  Jane Hsieh
		</span>
	  </NavBrand>
		<NavUl {activeUrl} {activeClass} {nonActiveClass}>
			<NavLi href="{base}/" class="text-lg">Home</NavLi>
			<!-- <NavLi href="{base}/research" class="text-lg">Research</NavLi>
			<NavLi href="{base}/cv" class="text-lg">CV</NavLi>
			<NavLi href="{base}/portfolio" class="text-lg">Portfolio</NavLi> -->
		</NavUl>
	</Navbar>

	<slot></slot>
</div>