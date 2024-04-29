<style>
  </body>#countdown {
    font-size: 36px;
    font-weight: bold;
    color: white;
    text-align: center;
    margin: 20px 0;
  }
</style>

<p id="countdown"></p>

<script>
  function updateCountdown() {
    let startTime = new Date("2023-02-28T15:22:00");
    const currentTime = new Date();
    let diffTime = startTime - currentTime;
    let totalSeconds = diffTime / 1000;

    while (totalSeconds <= 0) {
      startTime.setDate(startTime.getDate() + 7);
      diffTime = startTime - currentTime;
      totalSeconds = diffTime / 1000;
    }

    const days = Math.floor(totalSeconds / (24 * 60 * 60));
    const hours = Math.floor((totalSeconds % (24 * 60 * 60)) / (60 * 60));
    const minutes = Math.floor((totalSeconds % (60 * 60)) / 60);
    const seconds = Math.floor(totalSeconds % 60);

    document.getElementById("countdown").innerHTML = `${days}d ${hours}h ${minutes}m ${seconds}s`;
  }

  setInterval(updateCountdown, 1000);
</script>
