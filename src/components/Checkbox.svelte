<script>
    export let label = "Checkbox";
    export let checked = false;
  </script>
  
  <div class="checkbox-group">
    <input type="checkbox" id="checkbox" bind:checked={checked} />
    <label for="checkbox">{label}</label>
  </div>
  
  <style>
    .checkbox-group {
        width: 100%;
        max-width: 263px;
        height: 100%;
        max-height: 70px;
        display: flex;
        align-items: center;
        margin-bottom: 1.5rem;
        margin: 0 auto;
        margin-bottom: 50px;
    }
    input[type="checkbox"] {
      margin-right: 0.5rem;
      border-radius: 8px;
    }
    label {
      color: white;
    }
  </style>
  