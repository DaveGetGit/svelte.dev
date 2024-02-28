<script>
  import CustomButton from "./CustomButton.svelte";

  function handleClick() {
    alert("Clicked");
  }
</script>

<CustomButton on:click={handleClick} />
