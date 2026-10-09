<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ORCA Network // Crimson</title>
    <style>
        :root {
            --bg-primary: #08090d;
            --bg-secondary: #11131c;
            --accent: #ff2a2a; /* Bloodshot Crimson Red */
            --accent-glow: rgba(255, 42, 42, 0.4);
            --text-main: #ffffff;
            --text-muted: #6c7282;
        }

        body {
            margin: 0;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-primary);
            color: var(--text-main);
            overflow-x: hidden;
        }

        /* Centered Logo Branding Area */
        .brand-header {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 50px 20px 20px 20px;
            text-align: center;
        }

        .orca-logo-svg {
            width: 120px;
            height: 120px;
            filter: drop-shadow(0 0 15px var(--accent));
            animation: pulse-glow 3s infinite ease-in-out;
        }

        .brand-name {
            font-size: 48px;
            font-weight: 900;
            color: var(--text-main);
            letter-spacing: 8px;
            margin-top: 15px;
            margin-bottom: 5px;
            text-shadow: 0 0 10px var(--accent-glow);
        }

        @keyframes pulse-glow {
            0%, 100% { filter: drop-shadow(0 0 12px rgba(255, 42, 42, 0.5)); }
            50% { filter: drop-shadow(0 0 25px rgba(255, 42, 42, 0.9)); }
        }

        /* Proxy Search UI */
        .proxy-container {
            max-width: 750px;
            margin: 0 auto 40px auto;
            padding: 0 20px;
            text-align: center;
        }

        .proxy-bar {
            display: flex;
            background: var(--bg-secondary);
            border: 2px solid rgba(255, 255, 255, 0.05);
            border-radius: 30px;
            padding: 8px 15px;
            transition: 0.3s;
            box-shadow: 0 8px 32px rgba(0,0,0,0.4);
        }

        .proxy-bar:focus-within {
            border-color: var(--accent);
            box-shadow: 0 0 20px var(--accent-glow);
        }

        .proxy-bar input {
            flex: 1;
            background: transparent;
            border: none;
            outline: none;
            color: white;
            font-size: 16px;
            padding: 10px;
        }

        .proxy-bar button {
            background: var(--accent);
            color: #ffffff;
            border: none;
            padding: 10px 25px;
            border-radius: 20px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.2s;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .proxy-bar button:hover {
            transform: scale(1.03);
            box-shadow: 0 0 15px var(--accent);
        }

        /* Game Grid Layout */
        .main-layout {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }

        .section-title {
            color: var(--text-muted);
            text-transform: uppercase;
            font-size: 13px;
            letter-spacing: 2px;
            margin-bottom: 20px;
            border-left: 3px solid var(--accent);
            padding-left: 10px;
        }

        .game-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: 20px;
        }

        .game-card {
            background: var(--bg-secondary);
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid rgba(255,255,255,0.03);
            transition: 0.25s;
            cursor: pointer;
            text-align: center;
            padding-bottom: 15px;
        }

        .game-card:hover {
            transform: translateY(-4px);
            border-color: var(--accent);
            box-shadow: 0 6px 20px rgba(255, 42, 42, 0.15);
        }

        .game-thumbnail {
            height: 110px;
            background: #161924;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 38px;
        }

        .game-title {
            margin-top: 12px;
            font-weight: 600;
            font-size: 14px;
            color: #e1e3e6;
        }
    </style>
</head>
<body>

    <!-- Redesigned Cyber Orca Header -->
    <div class="brand-header">
        <svg class="orca-logo-svg" viewBox="0 0 100 100" fill="none" xmlns="http://w3.org">
            <!-- Sleek Geometric/Cyber Orca Silhouette Fin & Body -->
            <path d="M20 65C35 60 45 42 42 25C48 38 62 48 85 45C65 52 58 68 55 80C50 72 35 68 20 65Z" fill="#ff2a2a"/>
            <!-- Aggressive Cyber Eye Detail -->
            <polygon points="48,42 56,43 52,46" fill="#ffffff"/>
            <!-- Accent Tech Lines -->
            <line x1="25" y1="72" x2="45" y2="72" stroke="#ff2a2a" stroke-width="2" stroke-linecap="round"/>
        </svg>
        <div class="brand-name">ORCA</div>
    </div>

    <div class="proxy-container">
        <div class="proxy-bar">
            <input type="text" placeholder="Search unblocked web apps or enter proxy strings...">
            <button>Execute</button>
        </div>
    </div>

    <div class="main-layout">
        <div class="section-title">Network Index // Available Systems</div>
        <div class="game-grid">
            <div class="game-card"><div class="game-thumbnail">👾</div><div class="game-title">Retro Space</div></div>
            <div class="game-card"><div class="game-thumbnail">🧱</div><div class="game-title">Block Craft 2D</div></div>
            <div class="game-card"><div class="game-thumbnail">🚗</div><div class="game-title">Neon Racer</div></div>
            <div class="game-card"><div class="game-thumbnail">🐍</div><div class="game-title">Cyber Snake</div></div>
            <div class="game-card"><div class="game-thumbnail">🧩</div><div class="game-title">Grid Puzzle</div></div>
        </div>
    </div>

</body>
</html>
# index.html
orca-network
