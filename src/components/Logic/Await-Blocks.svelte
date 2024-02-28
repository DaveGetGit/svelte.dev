<script>
  let promise = getRandomNumber();

  async function getRandomNumber() {
    const res = await fetch(`https://csrng.net/csrng/csrng.php?min=0&max=100`);

    if (res.ok) {
      const data = await res.json();
      return data[0].random;
    } else {
      throw new Error(res);
    }
  }

  async function handleClick() {
    promise = await getRandomNumber();
  }
</script>

<button on:click={handleClick}> Generate random number</button>

{#await promise}
  <p>...waiting</p>
{:then number}
  <p>The number is {number}</p>
{:catch error}
  <p style="color:red">{error.message}</p>
{/await}
