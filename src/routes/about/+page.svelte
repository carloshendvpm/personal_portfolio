<script>
	import {
		Timeline,
		TimelineItem,
		TimelineSeparator,
		TimelineDot,
		TimelineConnector,
		TimelineContent,
		TimelineOppositeContent
	} from 'svelte-vertical-timeline';

	const options = [
		{ time: '2018 - 2020', title: 'Téc em Desenvolvimento de Sistemas - ETE PORTO DIGITAL' },
		{ title: 'Analise e Desenvolvimento de Sistemas - SENAC', time: '2021 - 2023' },
		{ title: 'Estagiário em Desenvolvimento Front-end - Secretária de Defesa Social PE', time: 'FEV 2022 - OUT 2022' },
		{ time: 'OUT 2022 - momento', title: 'Desenvolvedor em Real Seguro Viagem' }
	];
</script>

<Timeline position="alternate">
	{#each options as option}
		<TimelineItem>
			<TimelineOppositeContent slot="opposite-content">
				<p>{option.time}</p>
			</TimelineOppositeContent>
			<TimelineSeparator>
				<TimelineDot />
				<TimelineConnector />
			</TimelineSeparator>
			<TimelineContent>
				<h3>{option.title}</h3>
			</TimelineContent>
		</TimelineItem>
	{/each}
</Timeline>