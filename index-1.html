<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>GHAT-SAFE - Blind Curve Warning System</title>
<style>
body{font-family:Arial,sans-serif;margin:0;background:#f1f5f9;color:#17212b}
header{background:#173b5e;color:white;padding:20px;text-align:center}
.container{max-width:900px;margin:auto;padding:16px}
.card{background:white;padding:20px;margin-bottom:18px;border-radius:12px;box-shadow:0 2px 8px #0001}
label{display:block;margin-top:15px;font-weight:bold}
select,input,button{width:100%;padding:12px;margin-top:8px;border-radius:7px;border:1px solid #bbb;font-size:16px;box-sizing:border-box}
button{background:#1769aa;color:white;border:none;cursor:pointer;margin-top:15px}
.warning{background:#e5f6e9;padding:15px;border-left:6px solid green;margin-top:15px;font-weight:bold}
.caution{background:#fff0cc;border-color:orange}
.danger{background:#ffe0e0;border-color:red}
.road{background:#555;color:white;padding:35px 10px;text-align:center;border-radius:12px;line-height:2.5}
.car{display:inline-block;padding:8px 14px;border-radius:5px;background:#1686d9;margin:8px}
.car2{background:#e34d4d}
.small{color:#596777;font-size:13px}
</style>
</head>
<body>
<header>
<h1>GHAT-SAFE</h1>
<p>Software-Based Blind-Curve Warning System for Ghat Roads</p>
</header>
<div class="container">
<div class="card">
<h2>About the Project</h2>
<p>GHAT-SAFE is a software demonstration showing how warning messages may help drivers approach blind curves on ghat roads more carefully.</p>
<p class="small">Demonstration only. This software does not detect real vehicles or connect to live road sensors.</p>
</div>
<div class="card">
<h2>Warning Control Panel</h2>
<label for="scenario">Traffic Scenario</label>
<select id="scenario">
<option value="clear">Road Clear</option>
<option value="ahead">Vehicle Ahead</option>
<option value="risk">Possible Head-On Risk</option>
</select>
<label for="speed">Vehicle Speed (km/h)</label>
<input type="range" id="speed" min="0" max="80" value="30">
<p>Speed: <strong><span id="speedValue">30</span> km/h</strong></p>
<label for="visibility">Visibility</label>
<select id="visibility">
<option value="good">Good</option>
<option value="limited" selected>Limited</option>
<option value="poor">Poor</option>
</select>
<div id="warning" class="warning" role="status">CLEAR — DRIVE CAREFULLY</div>
<button id="speakButton">🔊 Speak Warning</button>
<button id="resetButton">Reset Demo</button>
</div>
<div class="card">
<h2>Ghat Road Simulation</h2>
<div class="road">
🏔️ Mountain Road<br>
<span class="car">🚙 Vehicle A</span>
<span class="car car2">🚗 Vehicle B</span><br>
⚠️ Blind Curve Ahead
</div>
<p class="small">Illustration only. Vehicles are not detected by cameras or sensors.</p>
</div>
<div class="card">
<h2>How It Works</h2>
<ol>
<li>Select a traffic scenario.</li>
<li>Adjust the demonstration speed.</li>
<li>Select visibility conditions.</li>
<li>Read the warning displayed by the software.</li>
<li>Tap Speak Warning to hear the message.</li>
</ol>
</div>
</div>
<script>
const scenario=document.getElementById("scenario");
const speed=document.getElementById("speed");
const visibility=document.getElementById("visibility");
const warning=document.getElementById("warning");
const speedValue=document.getElementById("speedValue");

function getWarningState(traffic,speed,visibility){
 if(traffic==="risk"){
  return {text:"DANGER: POSSIBLE HEAD-ON RISK. SLOW DOWN.",level:"danger"};
 }
 if(visibility==="poor" && speed>35){
  return {text:"DANGER: POOR VISIBILITY. REDUCE SPEED.",level:"danger"};
 }
 if(traffic==="ahead" || (visibility==="limited" && speed>40)){
  return {text:"CAUTION: VEHICLE AHEAD OR LIMITED VISIBILITY.",level:"caution"};
 }
 if(visibility==="poor"){
  return {text:"CAUTION: POOR VISIBILITY. DRIVE SLOWLY.",level:"caution"};
 }
 return {text:"CLEAR: DRIVE CAREFULLY.",level:"safe"};
}

function updateWarning(){
 const currentSpeed=Number(speed.value);
 speedValue.textContent=currentSpeed;
 const result=getWarningState(scenario.value,currentSpeed,visibility.value);
 warning.textContent=result.text;
 warning.className="warning";
 if(result.level==="caution") warning.classList.add("caution");
 if(result.level==="danger") warning.classList.add("danger");
}

document.getElementById("speakButton").addEventListener("click",function(){
 if(!("speechSynthesis" in window)){
  alert("Voice warnings are not supported in this browser.");
  return;
 }
 window.speechSynthesis.cancel();
 window.speechSynthesis.speak(new SpeechSynthesisUtterance(warning.textContent));
});

document.getElementById("resetButton").addEventListener("click",function(){
 scenario.value="clear";
 speed.value=30;
 visibility.value="limited";
 updateWarning();
});

scenario.addEventListener("change",updateWarning);
speed.addEventListener("input",updateWarning);
visibility.addEventListener("change",updateWarning);
updateWarning();
</script>
</body>
</html>
