<script>
  let answer = "";
  let selected;
  let questions = [
    { id: 1, text: `Where did you go to school?` },
    { id: 2, text: `What is your mother's name?` },
    {
      id: 3,
      text: `What is another personal fact that an attacker could easily find with Google?`,
    },
  ];

  function handleSubmit() {
    alert(`answered question ${selected.id} (${selected.text}) with ${answer}`);
  }
</script>

<h2>Insecurity Questions</h2>

<form on:submit|preventDefault={handleSubmit}>
  <select
    bind:value={selected}
    on:change={() => {
      answer = "";
    }}
  >
    {#each questions as question}
      <option value={question}>{question.text}</option>
    {/each}
  </select>

  <p><input bind:value={answer} /></p>

  <p>
    <button type="submit" disabled={!answer}>Submit</button>
  </p>
</form>

<p>selected question {selected ? selected.id : "Waiting..."}</p>
