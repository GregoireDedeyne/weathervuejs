<template>
	<div
		className="card w-64 bg-base-100 shadow-xl image-full carousel-item h-96 m-2"
	>
		<figure>
			<img
				src="https://daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg"
				alt="Shoes"
			/>
		</figure>
		<div className="card-body">
			<h2 className="card-title">{{ title }}!</h2>
			<p>{{ description }}</p>
			<div className="card-actions justify-end">
				<button className="btn btn-primary">Voir plus</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	props: ["title", "description"],
};
</script>
