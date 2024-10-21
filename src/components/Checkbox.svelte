<!-- Checkbox.svelte -->
<script>
    export let label = "";
    export let checked = false;
  </script>
  
  <div class="checkbox-group">
    <input type="checkbox" id="checkbox" bind:checked={checked} />
    <label for="checkbox">{label}</label>
  </div>
  
  <style>
    .checkbox-group {
      display: flex;
      align-items: center;
      margin-bottom: 1.5rem;
    }
    input[type="checkbox"] {
      margin-right: 0.5rem;
    }
    label {
      color: white;
    }
  </style>
  