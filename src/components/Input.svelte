<script>
  export let placeholder = "";
  export let required = false;
  export let value = "";
</script>

<div class="input-group">
  <input
    type="text"
    class="input"
    placeholder={placeholder}
    bind:value
    required={required}
  />
</div>

<style>
  .input-group {
    margin-bottom: 1rem;
  }
  .input {
    width: 100%;
    padding: 0.8rem;
    border-radius: 5px;
    border: 1px solid #ccc;
    background-color: #1e1e2e;
    color: white;
  }
  .input::placeholder {
    color: #ccc;
  }
</style>
