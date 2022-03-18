<template>
	<div class="home-view">
		<TopBar />
		<h1 class="h3 text-center">Brasileirão Série A</h1>
		<div id="conteudo" class="d-flex flex-column align-center">
			<v-img class="my-6" src="../assets/brasileirao-imagem.jpeg" />
			<p class="my-6 text-center px-2">
				A série A do campeonato Brasileiro de Futebol de 2020, oficialmente
				Brasileirão Açaí - Série A 2020 por motivos de patrocinio, é a 64º
				edição da priincipal divisão do futebol Brasileiro. A disputa tem o
				mesmo regulamento dos anos anteriores, quando foi implementado o sistema
				de pontos corridos.
			</p>
		</div>
	</div>
</template>

<script>
import TopBar from '../components/shared/TopBar.vue';
export default {
	name: 'HomeView',

	components: {
		TopBar,
	},
};
</script>
