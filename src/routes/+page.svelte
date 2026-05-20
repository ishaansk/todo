<script>
  let todos = $state([
    { text: "todo1", done: false },
    { text: "todo2", done: false },
  ]);
</script>

<div class="todos">
  {#each todos as todo, i}
    <div class="todo">
      <input bind:value={todo.text} type="text" />
      <input bind:checked={todo.done} type="checkbox" />
    </div>
  {/each}
</div>
