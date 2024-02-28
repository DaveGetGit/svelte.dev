<script>
  let m = { x: 0, y: 0 };

  function handleMouseMove(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }
</script>

<div on:mousemove={handleMouseMove} role="presentation">
  The mouse is on x: {m.x} and y: {m.y}
</div>
