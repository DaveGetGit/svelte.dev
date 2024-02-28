<script>
  let m = { x: 0, y: 0 };
</script>

<div
  role="presentation"
  on:mousemove={(e) => (m = { x: e.clientX, y: e.clientY })}
>
  The mouse is on x: {m.x} and y: {m.y}
</div>
