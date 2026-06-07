<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ARG FRAGMENT — Second Lives</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    background: #000000;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    font-family: 'Courier New', 'Fira Code', monospace;
    padding: 20px;
  }
  .arg-terminal {
    max-width: 750px;
    width: 100%;
    background: #0a0a0f;
    background-image: 
      linear-gradient(0deg, rgba(0,255,255,0.02) 1px, transparent 1px),
      linear-gradient(90deg, rgba(255,0,102,0.02) 1px, transparent 1px);
    background-size: 30px 30px;
    border: 1px solid #ff4d4d;
    border-radius: 28px;
    padding: 28px 26px;
    box-shadow: 
      0 0 30px rgba(255, 77, 77, 0.2),
      inset 0 0 40px rgba(0,0,0,0.5),
      0 20px 40px rgba(0,0,0,0.5);
    position: relative;
    transition: all 0.3s ease;
  }
  .arg-terminal::before {
    content: "";
    position: absolute;
    top: -2px;
    left: -2px;
    right: -2px;
    bottom: -2px;
    background: linear-gradient(45deg, #ff4d4d, #7df9ff, #ff4d4d, #7df9ff);
    border-radius: 30px;
    z-index: -1;
    opacity: 0.3;
    filter: blur(8px);
  }
  .arg-terminal::after {
    content: "⨯ BREACH // ACTIVE ⨯";
    position: absolute;
    bottom: -25px;
    right: 20px;
    font-size: 9px;
    color: #ff4d4d80;
    letter-spacing: 2px;
  }
  .glitch {
    font-size: 14px;
    font-weight: bold;
    color: #ff4d4d;
    text-shadow: 2px 0 0 #7df9ff, -2px 0 0 #ff0066;
    animation: glitch 1.2s infinite;
    display: inline-block;
  }
  @keyframes glitch {
    0% { text-shadow: 2px 0 0 #7df9ff, -2px 0 0 #ff0066; }
    50% { text-shadow: -2px 0 0 #7df9ff, 2px 0 0 #ff0066; }
    100% { text-shadow: 2px 0 0 #7df9ff, -2px 0 0 #ff0066; }
  }
  .badge {
    background: #ff4d4d20;
    border: 1px solid #ff4d4d60;
    border-radius: 60px;
    padding: 5px 15px;
    font-size: 11px;
    letter-spacing: 2px;
    display: inline-block;
    backdrop-filter: blur(4px);
  }
  .neon-text {
    color: #7df9ff;
    text-shadow: 0 0 5px #7df9ff, 0 0 1px #7df9ff;
  }
  .divider {
    height: 2px;
    background: linear-gradient(90deg, transparent, #ff4d4d, #7df9ff, #ff4d4d, transparent);
    margin: 22px 0;
    animation: pulseDiv 2s infinite;
  }
  @keyframes pulseDiv {
    0% { opacity: 0.5; }
    50% { opacity: 1; }
    100% { opacity: 0.5; }
  }
  .access-card {
    background: #0b0b0fd9;
    border-left: 4px solid #7df9ff;
    border-radius: 12px;
    padding: 14px 18px;
    margin: 15px 0;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .access-card:hover {
    transform: translateX(6px);
    box-shadow: -5px 0 15px rgba(125, 249, 255, 0.2);
  }
  .crew-box, .voice-box {
    background: #111116;
    border-radius: 16px;
    padding: 14px 18px;
    margin: 12px 0;
    border: 1px solid #2a2a35;
  }
  a {
    color: #7df9ff;
    text-decoration: none;
    font-weight: bold;
    transition: all 0.2s;
    display: inline-block;
  }
  a:hover {
    color: #ff4d4d;
    text-shadow: 0 0 5px #ff4d4d;
    transform: scale(1.02);
  }
  .cursor-blink {
    display: inline-block;
    width: 8px;
    height: 14px;
    background: #7df9ff;
    vertical-align: middle;
    animation: blink 1s step-end infinite;
    margin-left: 6px;
  }
  @keyframes blink {
    0%, 100% { opacity: 1; }
    50% { opacity: 0; }
  }
  .small-print {
    font-size: 9px;
    color: #444;
    text-align: center;
    margin-top: 25px;
    letter-spacing: 1px;
  }
  h4 {
    color: #ffcc66;
    font-size: 16px;
    margin-bottom: 8px;
    letter-spacing: 1px;
  }
</style>
</head>
<body>
<div class="arg-terminal">
  
  <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; margin-bottom: 16px;">
    <span class="badge">⚠️ CLASSIFIED // ARG FRAGMENT</span>
    <span style="color: #7df9ff; font-size: 12px;">[ v.2.3.1 // BREACH]</span>
  </div>

  <p><span class="glitch">⛔ [NOTICE]</span> <span style="color: #bcbcbc;">This is an</span> <strong class="neon-text">Alternate Reality Game</strong> <span style="color: #bcbcbc;">website.</span> <span style="color: #666;">Everything is fictional. Not real at all.</span></p>

  <div class="divider"></div>

  <h4>🔻 [PUZZLE ACCESS] — ENTER THE FRACTURE</h4>
  <div class="access-card">
    🧩 <a href="https://rojz23.github.io/SecondLives.html">&gt; Second Lives Corp website</a><br><br>
    ⚡ <a href="https://rojz23.github.io/BreachUnit.html">&gt; Breach Unit — unauthorized zone</a>
    <span class="cursor-blink"></span>
  </div>

  <h4>📁 [CREW FILE] // ACCESS: GRANTED</h4>
  <div class="crew-box">
    <span style="color: #aaa;">creator, writer, and ARG director:</span><br>
    <span style="color: #ffcc66; font-weight: bold; font-size: 17px;">✦ Rojina Z.</span> <span style="color: #888;">[ Dead Society ]</span>
  </div>

  <h4>🎙️ [VOICE CAST] — SIGNAL TRACE</h4>
  <div class="voice-box">
    <span style="color: #ff9999;">▸ Fahad Fade</span> <span style="color: #777;">— voice of Asher Vance</span><br>
    <span style="color: #ff9999;">▸ Katie Otten</span> <span style="color: #777;">— voice of Kira Daniels</span><br>
    <span style="color: #ff9999;">▸ Justice Margowski</span> <span style="color: #777;">— voice of General Nathaniel Keir</span>
  </div>

  <div class="divider" style="margin: 18px 0 12px;"></div>
  <div class="small-print">
    [ FRAGMENT // DO NOT TRUST // BREACH UNIT WATCHING ]<br>
    ⚡ <span style="color:#7df9ff;">SECOND LIVES CORP</span> ⚡ <span style="color:#ff4d4d;">BREACH UNIT</span> ⚡
  </div>
</div>
</body>
</html>
