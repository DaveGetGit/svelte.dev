<script>
  let flavours = ["Mint choc chip"];
  let scoops = 1;
  let menu = ["Cookies and Cream", "Mint choc chip", "Rasberry ripple"];

  function join(flavours) {
    if (flavours.length === 1) return flavours[0];
    return `${flavours.slice(0, -1).join(", ")} and ${
      flavours[flavours.length - 1]
    }`;
  }
</script>

<h2>Size</h2>

<label>
  <input type="radio" bind:group={scoops} value={1} />
  One Scoop
</label>
<label>
  <input type="radio" bind:group={scoops} value={2} />
  Two Scoops
</label>
<label>
  <input type="radio" bind:group={scoops} value={3} />
  Three Scoops
</label>

<h2>Flavours</h2>

{#each menu as flavour}
  <label>
    <input type="checkbox" bind:group={flavours} value={flavour} />
    {flavour}
  </label>
{/each}

{#if flavours.length === 0}
  <p>Please select at least one flavour</p>
{:else if flavours.length > scoops}
  <p>Cant order more flavours than scoops</p>
{:else}
  <p>
    You ordered {scoops} of {scoops === 1 ? "scoop" : "scoops"} of
    {join(flavours)}
  </p>
{/if}
