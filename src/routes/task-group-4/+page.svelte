<script>
	// [Task 1]
	// Import the `Nested.svelte` component so that the name matches line 19

	import Nested from "./Nested.svelte"
	
	// [Task 2]
	// Create a new component called MyInput.svelte inside this folder
	import MyInput from "./MyInput.svelte";

	// [Task 3]
	// Add a text input element inside your new component

	// [Task 4]
	// Make the borders of your MyInput component red

</script>

<p>These styles...</p>

<!-- Uncomment this `Nested` component below after completing [Task 1], make sure it works -->
<Nested/>
<MyInput/>
<!-- Put your new component here after doing [Task 2], [Task 3], and [Task 4] -->

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>