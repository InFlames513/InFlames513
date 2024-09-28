<div align="center">
  <h1>Hi! I'am InFlames</p><h1>
  <h2 id="discord_status"></h2>
  <h3>:man_technologist: I like Python and JavaScript.<br>:handshake: I share my made projects at github.<br>:star2: Don't forget to give stars to my projects.<br>:mending_heart: Good Work!</h3>
</div>

<script>
  setInterval(() => {
    fetch("https://api.lanyard.rest/v1/users/162969778699501569").then(res => {
      console.log(res.json());
      let data = res.json().data.discord_status;
      let status = data=="dnd"?"🔴 Do Not Disturb ":data=="idle"?"🟡 Idle":data=="online"?"🟢 Online":"⚪ Offline";
      document.getElementById("discord_status").innerHTML = status;
    });
  });
</script>
