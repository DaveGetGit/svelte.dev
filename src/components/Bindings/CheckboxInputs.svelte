<script>
  let yes = false;
</script>

<label>
  <input type="checkbox" bind:checked={yes} />
  Yes! Send me regular email sapm.
</label>

{#if yes}
  <p>Thank You</p>
{:else}
  <p>You must opt-in to continue.</p>
{/if}

<button disabled={!yes}>Subscribe</button>
