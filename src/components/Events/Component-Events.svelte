<script>
  import InnerComponent from "./InnerComponent.svelte";

  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<InnerComponent on:message={handleMessage} />
