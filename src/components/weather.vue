<template>
	<div class="m-2 text-black">
		<h1>{{ day }}</h1>
		<div>Emoji</div>
		<span>59° </span> <span> 59° </span>
	</div>
</template>

<script>
export default {
	props: ["day"],
};
</script>
