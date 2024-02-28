<script>
  let cats = [
    { id: "J---aiyznGQ", name: "Keyboard Cat" },
    { id: "z_AbfPXTKms", name: "Maru" },
    { id: "OUtn3pvWmpg", name: "Henri The Existensial Cat" },
  ];
</script>

<h1>The Famous Cats of Youtube</h1>

<ul>
  {#each cats as { id, name }, i}
    <li>
      <a
        target="_blanck"
        rel="noreferer"
        href="https://www.youtube.com/watch?v={id}"
      >
        {i + 1}:
        {name}
      </a>
    </li>
  {/each}
</ul>
