<script>
  let src = "assets/avatar.png";
  let arrowDown = "assets/arrow-down.svg";
</script>

<div class="avatar">
  <img {src} alt="Avatar" width="50" />
  <div class="info">
    <p>Easin Arafat</p>
    <p>SEO Specialist</p>
  </div>
  <div class="arrow_down">
    <img src={arrowDown} alt="Arrow down" width="8" />
  </div>
</div>

<style>
  .avatar p {
    color: #caccd6;
    margin: 0;
    font-family: "Arial";
  }

  .avatar {
    height: 50px;
    display: flex;
    align-items: center;
  }

  .avatar .info {
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }

  .avatar .info p {
    font-size: 14px;
    font-weight: 600;
    margin-left: 10px;
  }

  .avatar .info p:first-child {
    margin-bottom: 5px;
  }

  .avatar .info p:not(:first-child) {
    color: rgba(202, 204, 214, 0.4);
  }

  .avatar .arrow_down {
    width: 26px;
    height: 26px;
    border-radius: 50%;
    background-color: #2f3661;

    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 17px;
  }
</style>
