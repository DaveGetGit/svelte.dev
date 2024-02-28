<script>
  import OuterComponent from "./OuterComponent.svelte";

  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<OuterComponent on:message={handleMessage} />
