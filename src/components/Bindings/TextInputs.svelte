<script>
  $: name = "";
</script>

<input type="text" bind:value={name} placeholder="Enter Your Name" />

<p>Hello {name || "Stranger"}!</p>
