<template>
	<v-container class="grey lighten-5">
		<v-row justify="center">
			<h1>OWASP MULTILIDAE II</h1>
		</v-row>
		<v-row justify="center">
			<h5>WEB PWN IN MASS PRODUCTION</h5>
		</v-row>
		<v-row justify="center">
			<menu-navigator />
		</v-row>
	</v-container>
</template>

<script>
	import Menu from "@/components/Menu";
	export default {
		components: {
			"menu-navigator": Menu,
		},
		data: () => ({}),
	};
</script>
<style scoped></style>
