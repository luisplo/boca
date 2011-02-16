<template>
	<v-card class="my-5">
		<v-tabs>
			<!-- <v-tabs-slider color="teal lighten-3"></v-tabs-slider> -->
			<v-tab v-for="i in menu" :key="i" :href="'#tab-' + i">
				{{ i }}
			</v-tab>
		</v-tabs>
	</v-card>
</template>
<script>
	export default {
		data() {
			return {
				menu: [
					"Home",
					"Login / Register",
					"Toggle Hints",
					"Show Popup Hints",
					"Toggle Security",
					"Enforce SSL",
					"Reset DB",
					"View Log",
					"View Capture Data",
				],
			};
		},
	};
</script>
