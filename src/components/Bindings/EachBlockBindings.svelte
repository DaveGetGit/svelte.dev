<script>
  let todos = [
    { done: false, text: "sample 1" },
    { done: false, text: "sample 2" },
    { done: false, text: "sample 3" },
  ];

  function add() {
    todos = todos.concat({ done: false, text: "" });
  }

  function clearCompleted() {
    todos = todos.filter((t) => !t.done);
  }
  $: remaining = todos.filter((t) => !t.done).length;
</script>

<h3>Todos</h3>

{#each todos as todo}
  <div>
    <input type="checkbox" bind:checked={todo.done} />
    <input type="text" disabled={todo.done} bind:value={todo.text} />
  </div>
{/each}

<p>{remaining} remaining</p>

<button on:click={add}> Add New </button>
<button on:click={clearCompleted}> Clear Completed </button>
