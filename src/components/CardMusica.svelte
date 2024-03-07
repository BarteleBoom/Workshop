<script>
	export let Nomealbum;
	export let Artista;
	export let durata;
	export let anno;
	export let image;
</script>

<!--  -->
<div class="card_musica">
	<img alt="copertina del disco" src={image} />
	<p class="card_musica_disco">{Nomealbum}</p>
	<p>{Artista}</p>
	<div class="card_musica_footer">
		<p>{durata}</p>
		<p>{anno}</p>
	</div>
</div>

<!--  -->
<style>
	.card_musica {
		background-color: rgba(113, 202, 127, 0.838);
		width: 300px;
		border-radius: 20px;
		overflow: hidden;
		padding: 20px;
		color: rgb(1, 90, 90);
		font-family: Arial, Helvetica, sans-serif;
	}

	.card_musica_disco {
		font-size: 27px;
	}

	.card_musica_footer {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
	}
</style>
