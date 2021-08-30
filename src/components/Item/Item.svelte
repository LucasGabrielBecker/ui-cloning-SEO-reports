<script>
  export let src;
  export let label;
  export let active = false;
</script>

<div class:active>
  <img {src} alt={label} />
  <h2>{label}</h2>
</div>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;700&display=swap");

  div {
    display: flex;
  }
  .active h2 {
    font-weight: 600;
    color: #fff;
  }

  h2 {
    margin-left: 20px;
    color: #caccd6;
    font-weight: 300;
    font-family: "Poppins", sans-serif;
  }
</style>
