<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>ARG // Second Lives & Breach Unit</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: radial-gradient(circle at 10% 20%, #0a0f1e, #03060c);
      font-family: 'Segoe UI', 'Courier New', 'Lucida Sans Typewriter', monospace;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 2rem;
    }

    /* main container — glitchy, futuristic dossier feel */
    .arg-container {
      max-width: 780px;
      width: 100%;
      background: rgba(8, 12, 19, 0.68);
      backdrop-filter: blur(3px);
      border: 1px solid rgba(80, 210, 194, 0.35);
      border-radius: 2rem;
      box-shadow: 0 25px 40px -12px rgba(0, 0, 0, 0.6), 0 0 0 1px rgba(0, 255, 255, 0.1) inset;
      padding: 2rem 2rem 2.5rem;
      transition: all 0.2s ease;
    }

    /* cryptic header */
    .arg-header {
      text-align: center;
      margin-bottom: 2.5rem;
      border-bottom: 2px dashed #2c666e;
      padding-bottom: 1rem;
    }

    .arg-header h1 {
      font-size: 2rem;
      letter-spacing: 4px;
      text-transform: uppercase;
      font-weight: 500;
      background: linear-gradient(135deg, #b3f0e8, #4cc9f0);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      text-shadow: 0 0 6px rgba(0, 210, 200, 0.4);
      word-break: keep-all;
    }

    .arg-header .sub {
      font-family: monospace;
      color: #84b7bb;
      font-size: 0.8rem;
      margin-top: 0.5rem;
      letter-spacing: 1px;
      word-break: break-word;
    }

    /* ========= LINK BLOCKS ========= 
       each link becomes a card-like block, 
       one below another, with space between.
    */
    .arg-link-block {
      display: flex;
      flex-direction: column;
      gap: 2rem;   /* clean space between each link block */
      margin-top: 0.5rem;
    }

    /* entry style — each "link + description" unit */
    .entry {
      background: rgba(3, 10, 18, 0.7);
      border-left: 5px solid #26c5b3;
      padding: 1.2rem 1.5rem;
      border-radius: 1.2rem;
      transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s;
      backdrop-filter: blur(2px);
      box-shadow: 0 6px 14px rgba(0, 0, 0, 0.3);
    }

    .entry:hover {
      transform: translateY(-3px);
      border-left-color: #f0a6ff;
      box-shadow: 0 14px 26px -8px rgba(0, 255, 255, 0.2);
      background: rgba(7, 18, 28, 0.85);
    }

    /* actual link style — bold, futuristic, interactive */
    .entry a {
      font-size: 1.7rem;
      font-weight: 600;
      font-family: 'Segoe UI', 'Courier New', monospace;
      text-decoration: none;
      display: inline-block;
      margin-bottom: 0.6rem;
      letter-spacing: -0.3px;
      background: linear-gradient(120deg, #d6f0ff, #94dbff);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      transition: all 0.2s;
      text-shadow: 0 0 2px rgba(0,230,250,0.3);
      border-bottom: 1px dotted rgba(100, 210, 200, 0.4);
    }

    .entry a:hover {
      background: linear-gradient(135deg, #ffffff, #a0f0ff);
      background-clip: text;
      -webkit-background-clip: text;
      text-shadow: 0 0 8px #00ffff80;
      border-bottom-color: #f0f;
    }

    /* description paragraph style */
    .desc {
      color: #cbd5e6;
      font-size: 0.95rem;
      line-height: 1.45;
      margin-top: 0.5rem;
      font-family: 'Segoe UI', 'Fira Code', monospace;
      border-top: 1px solid rgba(70, 130, 130, 0.4);
      padding-top: 0.7rem;
      letter-spacing: 0.2px;
    }

    /* Extra ARG flavor elements */
    .glitch-note {
      margin-top: 2.8rem;
      text-align: center;
      font-size: 0.75rem;
      color: #6c94a0;
      border-top: 1px solid #1e464e;
      padding-top: 1.2rem;
      font-family: monospace;
      display: flex;
      justify-content: center;
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    .glitch-note span {
      background: #07161f;
      padding: 0.2rem 0.7rem;
      border-radius: 40px;
      font-size: 0.7rem;
      letter-spacing: 1px;
    }

    /* responsive: on smaller screens, font-size tweaks */
    @media (max-width: 550px) {
      .arg-container {
        padding: 1.4rem;
      }
      .entry a {
        font-size: 1.3rem;
        word-break: break-word;
      }
      .desc {
        font-size: 0.85rem;
      }
      .arg-header h1 {
        font-size: 1.5rem;
      }
    }

    /* custom cursor / immersive touch */
    a, .entry {
      cursor: pointer;
    }
  </style>
</head>
<body>
<div class="arg-container">
  <div class="arg-header">
    <h1>⌬ ECHO PROTOCOL ⌬</h1>
    <div class="sub">ALTERNATE REALITY GAME // ACCESS RESTRICTED NODES</div>
    <div class="sub" style="font-size:0.7rem; margin-top:6px;">▼  SIGNAL DETECTED  ▼</div>
  </div>

  <!-- 
    LINKS ONE BELOW ANOTHER + SPACING BETWEEN THEM
    each 'entry' contains a link + its immersive description
    pure semantic HTML with enhanced styling.
  -->
  <div class="arg-link-block">
    
    <!-- first link block : Second Lives Corp website -->
    <div class="entry">
      <a href="SecondLives.html" class="arg-link">⟡ Second Lives Corp website ⟡</a>
      <div class="desc">
        [//] ENTER THE CORPORATE MAZE: Second Lives Corp offers digital reincarnation — 
        consciousness uploading, identity masking, and memory harvesting. Unearth the 
        encrypted employee handbooks, lost testimonies, and hidden backdoors. Are you 
        a customer … or the product?<br>
        <span style="font-size:0.7rem; opacity:0.7;">⚡ core fragments: Rebirth protocol | shell accounts | data ghosts</span>
      </div>
    </div>

    <!-- second link block : Breach Unit -->
    <div class="entry">
      <a href="BreachUnit.html" class="arg-link">⛁ Breach Unit ⛁</a>
      <div class="desc">
        [//] OFFENSIVE CYBER DIVISION: join the rogue tactical squad that cracks reality 
        firewalls. Breach Unit operatives expose corrupted sim-layers and dismantle 
        corporate propaganda. Expect leaked field reports, anomaly casefiles, and 
        interactive signal intercepts.<br>
        <span style="font-size:0.7rem; opacity:0.7;">⚡ mission log: zero-day exploits | phantom gateways | dead drops</span>
      </div>
    </div>

  </div>

  <!-- optional flavor : immersive ARG footer / status -->
  <div class="glitch-note">
    <span>⚠️ UNSOLVED TRANSMISSION ⚠️</span>
    <span>🔒 clearance: omega</span>
    <span>📡 live data feed: active</span>
  </div>
</div>
</body>
</html>
