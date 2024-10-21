<script>
  export let placeholder = "";
  export let required = false;
  export let value = "";
</script>

<div class="input-group">
    <h3 class="input-title">{placeholder}</h3>
  <input
    type="text"
    class="input"
    bind:value
    required={required}
  />
</div>

<style>

    .input-title {
        font-size: 18px;
        text-align-last: left;
        color: #797EA3;
        width: 100%;
        max-width: 300px;
        margin: 0 auto 5px;
    }
  .input-group {
    max-height: 51px;
    height: 100%;
    margin-bottom: 1rem;
  }
  .input {
    padding-bottom: 6px;
    font-size: 18px;
    width: 100%;
    max-width: 300px;
    height: 22px;
    max-height: 51px;
    border: 0;
    border-bottom: 1px solid #3F4363;
    background-color: #171929;
    color: white;
    margin-bottom: 30px;
  }

  .input:focus {
    border: 0;
    border-bottom: 1px solid #FFF;
    outline-offset: 0px;
    outline: none;
  }

</style>
