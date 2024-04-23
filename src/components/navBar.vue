<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
	<div className="navbar bg-slate-200 text-black">
		<div className="navbar-start">
			<div className="dropdown">
				<div
					tabIndex="{0}"
					role="button"
					className="btn btn-ghost btn-circle"
				>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						className="h-5 w-5"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
					>
						<path
							strokeLinecap="round"
							strokeLinejoin="round"
							strokeWidth="2"
							d="M4 6h16M4 12h16M4 18h7"
						/>
					</svg>
				</div>
				<ul
					tabIndex="{0}"
					className="menu menu-sm dropdown-content mt-3 z-[1] p-2 shadow bg-slate-200 rounded-box w-52"
				>
					<li><RouterLink to="/"> Accueil</RouterLink></li>
					<li><RouterLink to="/login"> Se connecter </RouterLink></li>
					<li><RouterLink to="/subscribe">S'inscrire</RouterLink></li>
					<li><RouterLink to="/settings">Mon profil</RouterLink></li>
					<li><RouterLink to="/about">About</RouterLink></li>
				</ul>
			</div>
		</div>
		<div className="navbar-center">
			<RouterLink to="/" className="btn btn-ghost text-xl"
				>Météo</RouterLink
			>
		</div>
		<div className="navbar-end">
			<button className="btn btn-ghost btn-circle">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					className="h-5 w-5"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor"
				>
					<path
						strokeLinecap="round"
						strokeLinejoin="round"
						strokeWidth="2"
						d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
					/>
				</svg>
			</button>
		</div>
	</div>
</template>
