<script lang="ts">
	import Contact from "./Contact.svelte";
	import DogApi from "./dogAPI.svelte";
	import About from "./about.svelte";
	import Projects from "./projects.svelte";
	import Start from "./start.svelte";
	let shown = "Start";
	let array = ["Start", "Contact", "dogAPI", "Projects", "About"];
	const tabChange = (e) => {
		shown = e.detail;
	};
</script>

<body>
	<Start />
	<About />
	<Projects />
	<Contact />
	<DogApi />
</body>

<style>
	body {
		background: url(nasa.jpg) no-repeat center center fixed;
		background-size: cover;
		color: whitesmoke;
	}
</style>
