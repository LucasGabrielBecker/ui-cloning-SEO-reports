<script>
  export let percentage;
  export let sessions;
  export let src;
  export let label;

  let isPositive = percentage.includes("+");
</script>

<div class="container">
  <center>
    <div class="icons">
      <img {src} alt="icon" width="40" />
      <div
        class="percentage"
        style={`--variation-color: ${isPositive ? "#0c7f6a" : "#A51010"}`}
      >
        <span>{percentage}</span>
      </div>
    </div>
    <p class="session_label">{label}</p>
    <span class="session">{sessions}</span>
  </center>
</div>

<style>
  .container {
    width: 200px;
    height: 200px;
    background: linear-gradient(to bottom, #343c6b, #262b4b);
    border-radius: 60px;
    border: 1px solid #2b54e7;
    font-family: "Arial";
  }

  .container .icons {
    width: 70px;
    height: 70px;
    margin-top: 25px;
  }

  .icons {
    background: linear-gradient(to bottom, #191d38, #292f58);
    border-radius: 25px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;

    width: 70px;
    height: 70px;
  }

  .icons:before {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: -1;
    margin: -1px;
    border-radius: inherit;
    background: linear-gradient(
      to bottom,
      rgba(116, 116, 116, 0.774),
      rgba(85, 85, 85, 0)
    );
  }

  .icons:hover::before {
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: -1;
    margin: -1px;
    border-radius: inherit;
    background: linear-gradient(
      to bottom,
      rgb(116, 116, 116),
      rgba(85, 85, 85, 0)
    );
  }

  .percentage {
    width: 52px;
    height: 22px;
    background-color: var(--variation-color, #0c7f6a);
    border: 2px solid rgba(0, 0, 0, 0.8);
    border-radius: 40px;

    display: flex;
    justify-content: center;
    align-items: center;

    position: absolute;
    left: 50%;
    transform: translateX(-26px);
    bottom: -15px;
  }

  .percentage span {
    font-size: 12px;
    color: #fff;
  }

  .session_label {
    color: #caccd6;
    font-size: 14px;
    font-weight: 600;
    margin: 0;
    margin-top: 34px;
  }

  .session {
    font-size: 28px;
    color: #dbdce3;
    font-family: "Arial";
  }
</style>
