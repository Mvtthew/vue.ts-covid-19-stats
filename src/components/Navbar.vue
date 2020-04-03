<template>
	<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
		<div class="container">
			<a class="navbar-brand" href="/">COVID-19 Stats</a>
			<div class="ml-auto" id="navbarNav">
				<ul class="navbar-nav">
					<li class="nav-item active">
						<a class="nav-link" href="/">Home</a>
					</li>
				</ul>
			</div>
		</div>
	</nav>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class Navbar extends Vue {}
</script>