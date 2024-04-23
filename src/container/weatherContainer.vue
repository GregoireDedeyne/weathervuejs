<script setup>
import weather from "../components/weather.vue";
</script>

<template>
	<div class="flex-col mt-10 bg-black bg-opacity-10">
		<div class="text-black">logo <span> Hecq </span></div>

		<div class="flex justify-between">
			<weather day="Lundi" />
			<weather day="Mardi" />
			<weather day="Mercredi" />
			<weather day="Jeudi" />
			<weather day="Vendredi" />
		</div>
	</div>
</template>
