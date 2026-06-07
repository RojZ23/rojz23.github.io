<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ARG // FRACTURE ACCESS</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      background: radial-gradient(ellipse at 20% 30%, #0a0a0f 0%, #020205 100%);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Fira Code', 'Courier New', monospace;
      padding: 20px;
    }

    /* Glitch effect for main container */
    .terminal {
      max-width: 700px;
      width: 100%;
      background: rgba(8, 8, 14, 0.75);
      backdrop-filter: blur(8px);
      border: 1px solid rgba(255, 77, 77, 0.3);
      border-radius: 32px;
      padding: 32px 28px;
      box-shadow: 
        0 0 40px rgba(255, 77, 77, 0.15),
        0 0 10px rgba(125, 249, 255, 0.1),
        inset 0 1px 0 rgba(255, 255, 255, 0.05);
      transition: all 0.3s ease;
      animation: fadeIn 1.2s cubic-bezier(0.16, 1, 0.2, 1);
    }

    .terminal:hover {
      border-color: rgba(125, 249, 255, 0.5);
      box-shadow: 0 0 60px rgba(125, 249, 255, 0.1);
    }

    @keyframes fadeIn {
      0% {
        opacity: 0;
        transform: translateY(30px) scale(0.96);
      }
      100% {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    /* blinking cursor */
    .badge {
      background: rgba(255, 77, 77, 0.2);
      padding: 6px 14px;
      border-radius: 60px;
      font-size: 11px;
      letter-spacing: 2.5px;
      font-weight: 500;
      color: #ff4d4d;
      border: 1px solid rgba(255, 77, 77, 0.4);
      display: inline-block;
      backdrop-filter: blur(2px);
    }

    .glow-text {
      color: #7df9ff;
      text-shadow: 0 0 6px #7df9ff80;
    }

    .divider {
      height: 2px;
      background: linear-gradient(90deg, transparent, #ff4d4d, #7df9ff, #ff4d4d, transparent);
      margin: 22px 0;
      width: 100%;
    }

    .pulse-link {
      display: block;
      background: rgba(10, 10, 20, 0.6);
      padding: 14px 18px;
      border-left: 3px solid #7df9ff;
      border-radius: 16px;
      text-decoration: none;
      transition: all 0.2s ease;
      margin-bottom: 10px;
    }

    .pulse-link:hover {
      background: rgba(125, 249, 255, 0.08);
      border-left: 3px solid #ff4d4d;
      transform: translateX(6px);
    }

    .pulse-link span:first-child {
      color: #7df9ff;
      font-weight: bold;
      font-size: 16px;
    }

    .danger-link {
      border-left-color: #ff4d4d;
    }

    .danger-link span:first-child {
      color: #ff9999;
    }

    .section-title {
      font-size: 15px;
      font-weight: 700;
      letter-spacing: 1px;
      margin-top: 24px;
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .crew-card, .cast-card {
      background: rgba(26, 26, 31, 0.5);
      backdrop-filter: blur(4px);
      padding: 14px 18px;
      border-radius: 20px;
      border: 1px solid rgba(255, 204, 102, 0.2);
      transition: 0.2s;
    }

    .crew-card:hover, .cast-card:hover {
      border-color: rgba(255, 204, 102, 0.5);
      background: rgba(30, 30, 40, 0.6);
    }

    .voice-line {
      margin: 8px 0;
      font-family: monospace;
    }

    .voice-name {
      color: #ff9999;
      font-weight: 600;
    }

    .dim {
      color: #777;
    }

    .footer-signal {
      margin-top: 28px;
      padding-top: 16px;
      text-align: center;
      font-size: 10px;
      letter-spacing: 1.2px;
      border-top: 1px dashed #333;
      color: #4a4a55;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.3; }
    }

    .scan-line {
      width: 100%;
      height: 100%;
      background: linear-gradient(180deg, transparent, rgba(125, 249, 255, 0.02), transparent);
      pointer-events: none;
      animation: scan 6s linear infinite;
    }

    @keyframes scan {
      0% { transform: translateY(-100%); }
      100% { transform: translateY(100%); }
    }
  </style>
</head>
<body>
  <div class="terminal">
    <!-- glitchy top badge -->
    <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; margin-bottom: 16px;">
      <div class="badge">⚠️ [CLASSIFIED — ARG FRAGMENT]</div>
      <div style="font-size: 11px; color: #7df9ff80;">⚡ BREACH UNIT v.0x7F</div>
    </div>

    <!-- notice block -->
    <p style="margin: 12px 0 8px;">
      <strong style="color: #ff4d4d; font-size: 19px;">⛔ [NOTICE]</strong>
      <span style="color: #c0c0c0;"> This is an </span>
      <span class="glow-text" style="font-weight: bold;">Alternate Reality Game</span>
      <span style="color: #c0c0c0;"> website.</span>
      <span style="color: #777;"> Everything is fictional. Not real at all.</span>
    </p>

    <div class="divider"></div>

    <!-- PUZZLE ACCESS -->
    <div class="section-title">
      <span style="color: #7df9ff;">🔻 [PUZZLE ACCESS]</span>
      <span style="font-size: 10px; background: #00000050; padding: 2px 8px; border-radius: 20px;">ENTER THE FRACTURE</span>
    </div>

    <a href="https://rojz23.github.io/SecondLives.html" class="pulse-link" style="text-decoration: none;">
      <span>➤ Second Lives Corp website</span>
      <span style="display: block; font-size: 11px; color: #7df9ffaa; margin-top: 4px;">// reality subscription active</span>
    </a>

    <a href="https://rojz23.github.io/BreachUnit.html" class="pulse-link danger-link" style="text-decoration: none;">
      <span>⚡ ➤ Breach Unit — unauthorized</span>
      <span style="display: block; font-size: 11px; color: #ff9999aa; margin-top: 4px;">// warning: signal trace active</span>
    </a>

    <!-- CREW FILE -->
    <div class="section-title" style="margin-top: 32px;">
      <span style="color: #ffcc66;">📁 [CREW FILE]</span>
      <span style="font-size: 10px; background: #ffcc6620; padding: 2px 8px; border-radius: 20px;">ACCESS: GRANTED</span>
    </div>

    <div class="crew-card">
      <span style="color: #aaa; font-size: 12px;">creator, writer, and ARG director:</span><br>
      <span style="color: #ffcc66; font-size: 18px; font-weight: bold;">• Rojina Z.</span>
      <span style="color: #888;"> [ Dead Society ]</span>
    </div>

    <!-- VOICE CAST -->
    <div class="section-title" style="margin-top: 32px;">
      <span style="color: #ffcc66;">🎙️ [VOICE CAST]</span>
      <span style="font-size: 10px; background: #ffcc6620; padding: 2px 8px; border-radius: 20px;">SIGNAL TRACE</span>
    </div>

    <div class="cast-card">
      <div class="voice-line"><span class="voice-name">Fahad Fade</span> <span class="dim">— voice of Asher Vance</span></div>
      <div class="voice-line"><span class="voice-name">Katie Otten</span> <span class="dim">— voice of Kira Daniels</span></div>
      <div class="voice-line"><span class="voice-name">Justice Margowski</span> <span class="dim">— voice of General Nathaniel Keir</span></div>
    </div>

    <!-- cool terminal stats -->
    <div style="margin: 24px 0 0; display: flex; gap: 14px; flex-wrap: wrap; font-size: 11px;">
      <span style="background: #00000040; padding: 4px 12px; border-radius: 40px;">🕳️ FRAGMENT: omega</span>
      <span style="background: #00000040; padding: 4px 12px; border-radius: 40px;">🌀 NARRATIVE BLEED: active</span>
      <span style="background: #00000040; padding: 4px 12px; border-radius: 40px;">🔒 CLEARANCE: fragment</span>
    </div>

    <div class="footer-signal">
      [ FRAGMENT // DO NOT TRUST // BREACH UNIT WATCHING ]<br>
      <span style="font-size: 9px;">⟡ reality is a service agreement ⟡</span>
    </div>
  </div>
</body>
</html>
