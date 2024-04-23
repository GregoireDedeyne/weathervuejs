<script setup>
import dailyInfoCard from "../components/dailyInfoCard.vue";
</script>

<template>
	<div class="flex justify-center mt-10">
		<div className="w-64 carousel md:carousel-center md:w-auto rounded-box">
			<dailyInfoCard title="Dernière nouvellle" description="lorem" />
			<dailyInfoCard title="Dernière nouvellle" description="lorem" />
			<dailyInfoCard title="Dernière nouvellle" description="lorem" />
			<dailyInfoCard title="Dernière nouvellle" description="lorem" />
		</div>
	</div>
</template>
