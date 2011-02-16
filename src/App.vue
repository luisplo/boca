<template>
	<div id="app">
		<sidebar />
		<router-view />
		<Footer />
	</div>
</template>
<script>
	import Sidebar from "@/components/Sidebar";
	import Footer from "@/components/Footer";

	export default {
		components: {
			Sidebar,
			Footer,
		},
	};
</script>
