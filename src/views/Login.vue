<script setup>
import { onMounted, onUnmounted } from "vue";
import firebase from "firebase/compat/app";
import * as firebaseui from "firebaseui";
import firebaseConfig from "../../firebaseConfig";

firebase.initializeApp(firebaseConfig);
const ui = new firebaseui.auth.AuthUI(firebase.auth());

onMounted(() => {
	// Initialiser FirebaseUI si ce n'est pas déjà fait
	const uiConfig = {
		callbacks: {
			signInSuccessWithAuthResult: function (authResult, redirectUrl) {
				// Gérer la connexion réussie ici
				return true;
			},
			uiShown: function () {
				// L'interface utilisateur FirebaseUI est visible. Vous pouvez peut-être masquer un élément de chargement ici.
			},
		},
		signInFlow: "popup",
		signInSuccessUrl: "/", // Rediriger l'utilisateur après la connexion réussie
		signInOptions: [
			firebase.auth.EmailAuthProvider.PROVIDER_ID, // Activer l'authentification par e-mail
		],
		// Vous pouvez également définir d'autres options de configuration Firebase UI ici
	};
	ui.start("#firebaseui-auth-container", uiConfig);
});

onUnmounted(() => {
	if (ui) {
		ui.delete();
	}
});
</script>

<template>
	<div id="firebaseui-auth-container"></div>
	<!-- Ajoutez cet élément -->
</template>
