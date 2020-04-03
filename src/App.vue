<template>
	<div id="app">
		<Navbar></Navbar>
		<div class="container">
			<Summary class="mt-4" :data="summaryData"></Summary>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Navbar from "./components/Navbar.vue";
import Summary from "./components/Summary.vue";
import SummarySchema from "./models/SummarySchema";

@Component({
	components: { Navbar, Summary }
})
export default class App extends Vue {
	summaryData!: SummarySchema;

	created(): void {
		this.summaryData = {
			cases: 25,
			recovered: 51,
			deaths: 15
		};
	}
}
</script>

<style lang="sass">
@import "../node_modules/bootstrap/scss/bootstrap.scss"
</style>