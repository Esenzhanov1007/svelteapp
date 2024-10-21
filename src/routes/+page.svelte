<script>
  import DataForm from '../components/DataForm.svelte';
</script>
  <div class="bg"></div>
  <DataForm />

  
<style>
    :global(*) {
        margin: 0;
        box-sizing: border-box;
    }

    .bg {
        position: fixed;
        top: 0;
        left: 0;
        z-index: -1;
        min-width: 100vw;
        min-height: 100vh;
        background-image: url('../assets/bg.jpeg');
    }
</style>