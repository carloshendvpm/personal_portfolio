<svelte:head>
	<title>Home</title>
	<meta name="description" content="carloshendvpm - portfolio" />
</svelte:head>

<div class="wrapper flex flex-col max-w-3xl my-0 mx-auto py-10 items-center px-5">
	<div class="flex items-center w-full justify-between">
		<div class="header flex flex-col h-full">
			<p class="text-white text-xl ">Olá pessoas, meu nome é</p>
			<p class="text-7xl text-white font-bold leading-snug ">Carlos<br>Henrique</p>
		</div>
		<div class="">
			<img class="h-64" src="./carlos.png" alt="">
		</div>
	</div>
	<div class="text-white text-xl mt-2">
		<p>
			Desenvolvedor Front-end atuando em projetos com ReactJs, HTML, Css, TypeScript, Js desde o fim de 2020. Pude atingir milhares de pessoas com projetos tanto como estagiário, como Freelancer,
	sempre prezando pela melhor experiência do usuário.
		</p>
	</div>
	<div class="flex item-start justify-between w-full mt-8">
		<ul class="flex flex-row gap-9">
			<li><a href=""><i class="fa fa-github" style="font-size:48px;color:white;"></i></a></li>
			<li><a href=""><i class="fa fa-linkedin" style="font-size:48px;color:white;"></i></a></li>
			<li><a href=""><i class="fa fa-instagram" style="font-size:48px;color:white;"></i></a></li>
			<li><a href=""><i class="fa fa-envelope" style="font-size:48px;color:white;"></i></a></li>
		</ul>
		<button class="bg-white rounded-md font-bold text-xs w-44">Trabalhe comigo</button>
	</div>
</div>

<style>
	i:hover {
		transition: 0.25s ease;
		color: #5F5F5F !important;
	}
</style>