<template>
	<v-card height="400px">
		<v-footer absolute :padless="true">
			<v-card flat tile width="100%" class="red lighten-1 text-center">
				<v-divider></v-divider>

				<v-card-text class="white--text">
					{{ new Date().getFullYear() }} — <strong>Vuetify</strong>
				</v-card-text>
			</v-card>
		</v-footer>
	</v-card>
</template>
<script>
	export default {
		data: () => ({
			icons: ["mdi-home", "mdi-email", "mdi-calendar", "mdi-delete"],
			items: ["default", "absolute", "fixed"],
			padless: false,
			variant: "default",
		}),
		computed: {
			localAttrs() {
				const attrs = {};

				if (this.variant === "default") {
					attrs.absolute = false;
					attrs.fixed = false;
				} else {
					attrs[this.variant] = true;
				}
				return attrs;
			},
		},
	};
</script>
