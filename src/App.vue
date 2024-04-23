<script setup>
import navBar from "./components/navBar.vue";

import footerC from "./components/footerC.vue";
</script>

<template>
	<div class="bg-fond-one bg-cover h-screen pt-10 flex flex-col">
		<div class="container mx-auto flex"><navBar /></div>
		<router-view />
		<div class="container mx-auto flex"><footerC /></div>
	</div>
</template>
