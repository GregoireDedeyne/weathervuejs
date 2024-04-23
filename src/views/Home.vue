<script setup>
import weatherContainer from "../container/weatherContainer.vue";
import dailyInfoCardSwipper from "../container/dailyInfoCardSwipper.vue";
</script>

<template>
	<div class="container mx-auto flex flex-col flex-grow">
		<weatherContainer />
		<dailyInfoCardSwipper />
	</div>
</template>
