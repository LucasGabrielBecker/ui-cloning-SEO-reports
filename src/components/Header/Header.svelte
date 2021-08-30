<script>
  import ReportButton from "../ReportButton/ReportButton.svelte";
  import Avatar from "../Avatar/Avatar.svelte";
</script>

<div class="header">
  <div class="logo">
    <span><strong>SEO</strong> Dashboard</span>
    <h5>itobd.com</h5>
  </div>
  <div class="top-right">
    <ReportButton />
    <Avatar />
  </div>
</div>

<style>
  .header {
    font-family: "Arial";
    display: flex;
    justify-content: space-between;
  }
  strong {
    color: #fff;
  }
  span {
    color: #caccd6;
  }
  h5 {
    margin: 0;
    margin-top: 10px;
    color: #caccd6;
    font-size: 17px;
  }

  .top-right {
    width: 400px;
    display: flex;
    justify-content: space-between;
  }
</style>
