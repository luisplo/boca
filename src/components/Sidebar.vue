<template>
	<v-app id="inspire">
		<v-navigation-drawer
			v-model="drawer"
			app
			class="pt-4"
			color="grey lighten-3"
			mini-variant
		>
		</v-navigation-drawer>
		<v-main>
			<router-view />
			<Footer />
		</v-main>
	</v-app>
</template>

<script>
	import Footer from "@/components/Footer";

	export default {
		components: {
			Footer,
		},
	};
</script>
