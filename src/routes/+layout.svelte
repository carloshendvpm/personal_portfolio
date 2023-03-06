<script>
	import { page } from '$app/stores'
	import { t, locale } from "../i18n";
	import "../app.css"
	
	function setLocale(){
		locale.set('en')
	}
	function setLocalePT(){
		locale.set('ptBR')
	}
</script>

<nav class="flex justify-between max-w-7xl my-0 mx-auto py-4 text-white px-4 ">
	<div class="logo">
		<h1>CHdev</h1>
	</div>
	<ul class="flex gap-4">
		<li>
			<a class=" p-1.5 rounded-sm ease-in duration-300 hover:bg-[#434343] {$page.url.pathname == '/' ? 'selected' : ''} " href="/">Home</a>
		</li>
		<li>
			<a class=" hover:bg-[#434343] p-1.5 rounded-sm ease-in duration-300 {$page.url.pathname == '/projects' ? 'selected' : ''}  " href="/projects">{$t("homepage.navprojects")}</a>
		</li>
		<li>
			<a class="hover:bg-[#434343] p-1.5 rounded-sm ease-in duration-300 {$page.url.pathname == '/about' ? 'selected' : ''} " href="/about">{$t("homepage.navabout")}</a>
		</li>
	</ul>
	<div>
		<button on:click={setLocalePT}>PT</button>
		<span>|</span>
		<!-- salvar essa info no localstorage -->
		<button on:click={setLocale}>EN</button>
	</div>
</nav>
<div class="divider border-b-2 border-[#929292]">
	
</div>
<slot />
<style lang="postcss">
	:global(html){
		background-color: theme(colors.zinc.800);
	}

	.selected {
		background-color: #434343;
		color: white;
	}
</style>