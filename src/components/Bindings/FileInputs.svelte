<script>
  let files;
</script>

<label for="avatar">
  <input type="file" accept="Image/jpg, Image/jpeg ,pdf" bind:files />
</label>
<br /><br />
<label for="many">
  <input type="file" bind:files multiple />
</label>

<h3>Selected Files</h3>
{#if files}
  {#each Array.from(files) as file}
    <p>{file.name} ({file.size} bytes)</p>
  {/each}
{/if}
