<template>
	<div>
		<v-card class="mx-auto overflow-hidden">
			<v-system-bar color="deep-purple darken-3"></v-system-bar>

			<v-app-bar color="deep-purple accent-4" dark>
				<v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
				<v-toolbar-title>Campeonato Brasileiro</v-toolbar-title>

				<v-spacer></v-spacer>
			</v-app-bar>
		</v-card>

		<v-navigation-drawer v-model="drawer" bottom temporary>
			<v-list nav dense>
				<v-list-item-group
					v-model="group"
					active-class="deep-purple--text text--accent-4"
				>
					<v-list-item>
						<v-list-item-title>
							<v-icon small>mdi-home</v-icon>
							<span>Inicio</span>
						</v-list-item-title>
					</v-list-item>

					<v-list-item>
						<v-list-item-title>
							<v-icon small>mdi-podium</v-icon> Classificação
						</v-list-item-title>
					</v-list-item>
				</v-list-item-group>
			</v-list>
		</v-navigation-drawer>
	</div>
</template>

<script>
export default {
	data: () => ({
		drawer: false,
		group: null,
	}),

	watch: {
		group() {
			this.drawer = false;
		},
	},
};
</script>
