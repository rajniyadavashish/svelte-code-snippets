<script lang="ts">
	// state rune
	let num = $state(0);
	// derived rune
	let userInfo = $derived(num === 0 ? 'Please click the button' : `you clicked ${num} times`);
	// we can also use functions in derived runes

	function onClick() {
		num++;
	}
</script>

<button onclick={onClick}>Click me</button>

<h1>{num}</h1>
<p>{userInfo}</p>
<div class="container">
	<p>this is left side</p>
	<p>this is right side</p>
</div>

<style>
	h1 {
		color: blue;
	}

	.container {
		display: flex;
		justify-content: space-between;
	}
</style>
