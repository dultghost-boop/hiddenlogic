# hiddenlogic
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>hiddenlogic_1 // Cyber Dev</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>

    <div class="glow-bg"></div>

    <div class="container">
        <header>
            <div class="logo">hl_<span class="neon">01</span></div>
            <div class="status"><span class="dot"></span> Online</div>
        </header>

        <main>
            <div class="profile-section">
                <img src="https://images.unsplash.com/photo-1607604276583-eef5d076aa5f?q=80&w=500" alt="Anime Dev" class="anime-profile">
                <h1>hiddenlogic_1</h1>
                <p class="bio">// Independent Software Engineer operating from the shadows.</p>
            </div>

            <div class="console">
                <div class="console-nav"><span class="c-dot r"></span><span class="c-dot y"></span><span class="c-dot g"></span></div>
                <div class="console-body">
                    <p><span class="dash">$</span> init --project anime-logic</p>
                    <p class="gray">> Loading neural networks... Success.</p>
                </div>
            </div>

            <div class="links-grid">
                <a href="https://instagram.com/اسم_حسابك" class="link-card">Instagram _</a>
                <a href="#" class="link-card">GitHub Repository _</a>
                <a href="#" class="link-card">Projects Grid _</a>
            </div>
        </main>

        <footer>
            <p>&copy; 2026 hiddenlogic_1. Built for the next gen.</p>
        </footer>
    </div>

</body>
</html>
:root {
    --bg: #050508;
    --card-bg: rgba(15, 15, 25, 0.7);
    --neon-cyan: #00f3ff;
    --text: #f0f0f5;
    --muted: #6e6e7e;
}

* { margin: 0; padding: 0; box-sizing: border-box; }
body {
    background-color: var(--bg);
    color: var(--text);
    font-family: 'Fira Code', monospace;
    display: flex;
    justify-content: center;
    padding: 40px 20px;
    min-height: 100vh;
    position: relative;
    overflow-x: hidden;
}

.glow-bg {
    position: absolute;
    top: -10%; left: 50%; transform: translateX(-50%);
    width: 600px; height: 600px;
    background: radial-gradient(circle, rgba(0,243,255,0.08) 0%, rgba(0,0,0,0) 70%);
    z-index: -1;
}

.container { width: 100%; max-width: 450px; }

header {
    display: flex; justify-content: space-between; align-items: center;
    margin-bottom: 40px; padding-bottom: 15px; border-bottom: 1px solid #151525;
}
.logo { font-weight: 700; font-size: 1.2rem; }
.neon { color: var(--neon-cyan); text-shadow: 0 0 10px var(--neon-cyan); }

.status { font-size: 0.8rem; color: var(--muted); display: flex; align-items: center; gap: 6px; }
.dot { width: 8px; height: 8px; background: #39ff14; border-radius: 50%; box-shadow: 0 0 8px #39ff14; }

.profile-section { text-align: center; margin-bottom: 30px; }
.anime-profile {
    width: 110px; height: 110px; border-radius: 24px;
    border: 2px solid var(--neon-cyan); object-fit: cover;
    box-shadow: 0 8px 24px rgba(0, 243, 255, 0.2); margin-bottom: 15px;
}
.profile-section h1 { font-size: 1.6rem; margin-bottom: 8px; letter-spacing: -1px; }
.bio { font-size: 0.85rem; color: var(--muted); line-height: 1.5; }

.console {
    background: var(--card-bg); border: 1px solid #1a1a30;
    border-radius: 12px; padding: 15px; margin-bottom: 30px; backdrop-filter: blur(10px);
}
.console-nav { display: flex; gap: 6px; margin-bottom: 10px; }
.c-dot { width: 8px; height: 8px; border-radius: 50%; }
.r { background: #ff5f56; } .y { background: #ffbd2e; } .g { background: #27c93f; }
.console-body { font-size: 0.8rem; }
.dash { color: var(--neon-cyan); }
.gray { color: var(--muted); margin-top: 5px; }

.links-grid { display: flex; flex-direction: column; gap: 12px; }
.link-card {
    background: var(--card-bg); border: 1px solid #151525;
    padding: 16px; border-radius: 12px; text-decoration: none;
    color: var(--text); font-size: 0.9rem; font-weight: bold;
    transition: all 0.3s; display: flex; justify-content: space-between;
}
.link-card:hover { border-color: var(--neon-cyan); background: rgba(0, 243, 255, 0.02); }

footer { text-align: center; margin-top: 50px; font-size: 0.7rem; color: var(--muted); }
