<template>
	<div id="app">
		<div id="main">
			<Header />
			<nuxt />
		</div>
		<Footer />
	</div>
</template>

<script>
import Header from '../components/Header';
import Footer from '../components/Footer';
export default {
	components: { Header, Footer }
};
</script>

<style>
:root {
	--background-color: black;
	--text-color: white;
	--accent-color: yellow;
}
.accented {
	color: var(--accent-color);
}
* {
	box-sizing: border-box;
	margin: 0;
	padding: 0;
}
html,
body,
#app {
	background: var(--background-color);
	color: var(--text-color);
	height: 100vh;
}
#app {
	display: flex;
	flex-direction: column;
	font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
#main {
	flex: 1 0 auto;
	width: 100%;
}
footer {
	margin-top: auto;
}
.container {
	margin: auto;
	overflow: hidden;
	width: 80%;
}
</style>
