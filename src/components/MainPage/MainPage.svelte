<script>
  import Header from "../Header/Header.svelte";
  import ItemMedidor from "../ItemMedidor/ItemMedidor.svelte";
</script>

<section>
  <Header />
  <div class="medidors">
    <ItemMedidor
      src="assets/speed.svg"
      label="Sessions"
      sessions="3.4M"
      percentage="-6.4%"
    />
    <ItemMedidor
      src="assets/visitors.svg"
      sessions="1.9M"
      label="Unique Visitors"
      percentage="+12.2%"
    />
    <ItemMedidor
      src="assets/speed.svg"
      label="Page speed"
      sessions="3.4M"
      percentage="-3.6%"
    />
    <ItemMedidor
      src="assets/visitors_duration.svg"
      label="Avg Visit duration"
      sessions="12.9"
      percentage="+4.8%"
    />
    <ItemMedidor
      src="assets/bouce_rate.svg"
      label="Bounce Rate"
      sessions="12.9"
      percentage="+4.8%"
    />
  </div>
</section>

<style>
  section {
    width: 100%;
    padding: 50px;
    font-size: 35px;
  }

  .medidors {
    display: flex;
    width: 100%;
    justify-content: space-evenly;
    margin-top: 20px;
  }
</style>
