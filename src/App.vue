<template>
	<div id="app">
		<navbar></navbar>
		<div class="container">
			<p>HA</p>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Navbar from "./components/Navbar.vue";

@Component({
	components: { Navbar }
})
export default class App extends Vue {}
</script>

<style lang="sass">
@import "../node_modules/bootstrap/scss/bootstrap.scss"
</style>