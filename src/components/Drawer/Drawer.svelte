<script>
  import Item from "../Item/Item.svelte";
</script>

<section>
  <h2>VERT</h2>
  <Item src="assets/blue_icon.svg" label="Dashboard" active />
  <Item src="assets/realtime.svg" label="Realtime" />
  <Item src="assets/audience.svg" label="Audience" />
  <Item src="assets/convertions.svg" label="Convertions" />
  <Item src="assets/settings.svg" label="Settings" />
</section>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;700&display=swap");
  section {
    height: 100vh;
    width: 270px;
    display: flex;
    justify-content: flex-start;
    flex-direction: column;
    padding-left: 20px;
    border-radius: 15%;
    border-right: 1px solid #fff;
  }

  h2 {
    color: #fff;
    font-weight: 200;
    font-family: "Poppins", sans-serif;
  }
</style>
