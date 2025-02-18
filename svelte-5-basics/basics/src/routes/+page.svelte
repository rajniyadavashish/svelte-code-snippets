<script lang="ts">
	function onClick() {
		console.log('The button has been clicked');
	}
  let num = 5;
</script>

<button onclick={onClick}>Click me</button>

<h1>{num}</h1>

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