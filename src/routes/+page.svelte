<script>
	import { t, locale, locales } from "../i18n";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="carloshendvpm - portfolio" />
</svelte:head>

<div class="wrapper flex flex-col max-w-3xl my-0 mx-auto py-20 items-center px-5">
	<div class="flex items-center w-full justify-between">
		<div class="header flex flex-col h-full">
			<p class="text-white text-xl">{$t("homepage.title")}</p>
			<p class="text-7xl text-white font-bold leading-snug ">Carlos<br>Henrique</p>
		</div>
		<div class="">
			<img class="h-64" src="./carlos.png" alt="">
		</div>
	</div>
	<div class="text-white text-xl mt-2">
		<p>
			{$t("homepage.text")}
		</p>
	</div>
	<div class="flex item-start justify-between w-full mt-8">
		<ul class="flex flex-row gap-9">
			<li><a href="https://github.com/carloshendvpm"><i class="fa fa-github" style="font-size:48px;color:white;"></i></a></li>
			<li><a href="https://www.linkedin.com/in/carloshenriquedvpm/"><i class="fa fa-linkedin" style="font-size:48px;color:white;"></i></a></li>
			<li><a href="https://www.linkedin.com/in/carloshenriquedvpm/"><i class="fa fa-instagram" style="font-size:48px;color:white;"></i></a></li>
			<li><a href="gmail.com"><i class="fa fa-envelope" style="font-size:48px;color:white;"></i></a></li>
		</ul>
		<button class="bg-white rounded-md font-bold text-sm w-44 transition duration-300 ease-out hover:bg-[#5F5F5F] ease-in">{$t("homepage.button")}</button>
	</div>
</div>

<style>
	i { 
		transition: 0.3s ease-in-out;
	}
	i:hover {
		color: #5F5F5F !important;
	}
</style>