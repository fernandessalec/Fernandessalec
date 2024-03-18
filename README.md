### Salve quebrada! 👋

<div align="center">
    <a href="https://github.com/fernandessalec">
  <img height="165em" src="https://github-readme-stats.vercel.app/api?username=fernandessalec&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true"/>
  <img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=fernandessalec&layout=compact&langs_count=7&theme=tokyonight"/>
</div>



<!DOCTYPE html>
<html>
<head>
<title>Digital Analog Clock</title>
<style>
#clock {
width: 200px;
height: 200px;
border: 10px solid #333;
border-radius: 50%;
margin: 50px auto;
position: relative;
}
#hour, #minute, #second {
position; absolute;
width: 50%;
height: 2px;
background: #333;
top:50%;
transform-origin: 100%;
transition: all 0.5s;
}
#hour {
background: #333;
}
#minute {
background: #666;
}
#second {
background: #f00;
}
</style>
</head>
<body>
<div id="clock">
<div id="hour></div>
<div id="minute"></div>
</div>
<script>
setInterval(uptadeClock, 1000);
function uptadeClock() {
let date = new Date();
let hours = date.getHours() % 12;
let minutes = date.getMinutes();
let seconds = date.getSeconds();
let hourDeg = (hours * 30) + (0.5 * minutes);
let minuteDeg = (minutes * 6) + (0.1 * seconds);
let secondDeg = seconds * 6;

document.getElementByld('hour').style.transform = `rotate(${hourDeg}deg)`;

document.getElementByld('minute').style.tranform = `rotate(${minuteDeg}deg)`;

document.getElementByld('second').style.tranform = `rotate(${secondDeg}deg)`;
}
</script>
</div>
<script>
setInterval(uptadeClock, 1000);
function uptadeClock(){
let date = new Date();
let hours = date.getHours() % 12;
let minutes = date.getMinutes();
let seconds = date.getSeconds();
let hourDeg = (hours * 30) + (0.5 * minutes);
let minuteDeg = (minutes * 6) + (0.1 * seconds);
let secondDeg = seconds *6;

document.getElementByld('hour').style.tranform = `rotate(${hourDeg}deg)`;

document.getElementByld('minute').style.tranform = `rotate(${secondDeg}deg)`;
}
</script>
</body>
</html>