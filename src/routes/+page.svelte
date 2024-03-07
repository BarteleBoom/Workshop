<script>
	import Cardmusica from '$components/CardMusica.svelte';
	//
	let dischi = [
		{
			artista: 'Grondante',
			Nomealbum: 'Hola',
			durata: '2h',
			anno: '2025',
			image:
				'https://assets.culturabologna.it/0e99cf30-73ea-4f91-a6b0-93162ed65392-vicko-mozara-m82uh-vamhg-unsplash.jpg/658e92357ddaf83a37526e47323880e7e339b4c0.jpg'
		},
		{
			artista: 'Geopardo',
			Nomealbum: 'Cespugli',
			durata: '3:00',
			anno: '2030',
			image: 'https://secret-garden.it/wp-content/uploads/2018/09/Cespuglio-sempreverde.jpg'
		},
		{
			artista: 'Dante',
			Nomealbum: 'Angeli',
			durata: '0:00',
			anno: '1999',
			image: 'https://romeartweek.com/images/event/CE-2970-0862-0.jpg'
		}
	];
</script>

<!--  -->
<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tailwindcss@3.4.1/src/css/preflight.css" />
</svelte:head>
<!--  -->
{#each dischi as disco}
	<Cardmusica
		Nomealbum={disco.Nomealbum}
		Artista={disco.artista}
		durata={disco.durata}
		anno={disco.anno}
		image={disco.image}
	/>
{/each}

<Cardmusica
	Nomealbum="Calendula"
	Artista="Grondante"
	durata="2:06"
	anno="2020"
	image="https://www.lerboristeria.com/imgs/erbario/foto/calendula.jpg"
/>
