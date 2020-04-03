<template>
	<div class="card">
		<div class="card-header">
			<h4>Summary stats</h4>
		</div>
		<div class="card-body">
			<div v-if="data">
				<p class="m-0">Total cases: {{data.cases}}</p>
				<p class="m-0">Recovered: {{data.recovered}}</p>
				<p class="m-0">Deaths: {{data.deaths}}</p>
			</div>
			<div v-else>
				<p class="m-0">Loading...</p>
			</div>
		</div>
	</div>
</template>

<script lang="ts">
import { Vue, Component, Prop } from "vue-property-decorator";
import SummarySchema from "../models/SummarySchema";
@Component
export default class Summary extends Vue {
	@Prop() data!: SummarySchema;
}
</script>