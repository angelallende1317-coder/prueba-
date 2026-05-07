<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Córdoba Capital RP | Oficial</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --cba-rojo: #C83338;
            --cba-blanco: #FFFFFF;
            --cba-azul: #006699;
            --accent: #ffca28;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: #000;
            color: white;
            margin: 0;
            overflow-x: hidden;
        }

        /* FONDO CON TU FOTO DE LA BANDERA */
        .hero-bg {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('bandera.jpg');
            background-size: cover;
            background-position: center;
            z-index: -1;
        }

        /* STICKERS FLOTANTES */
        .sticker-v {
            position: fixed;
            z-index: 1000;
            display: flex;
            flex-direction: column;
            align-items: center;
            animation: float 5s ease-in-out infinite;
        }
        .fernet-v { bottom: 30px; left: 30px; color: #3d1b10; transform: rotate(-15deg); }
        .coca-v { top: 30px; right: 30px; color: #e41e26; transform: rotate(15deg); }
        
        .sticker-label {
            font-size: 0.7rem; background: white; color: black; padding: 2px 8px;
            border-radius: 5px; margin-top: -10px; border: 2px solid black; font-weight: 900;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0) rotate(-10deg); }
            50% { transform: translateY(-20px) rotate(10deg); }
        }

        header {
            height: 55vh; display: flex; flex-direction: column;
            justify-content: center; align-items: center; text-align: center; padding: 20px;
        }

        .titulo-cba {
            font-size: clamp(3rem, 10vw, 6rem); font-weight: 900; margin: 0;
            background: linear-gradient(to right, var(--cba-rojo) 33%, var(--cba-blanco) 33%, var(--cba-blanco) 66%, var(--cba-azul) 66%);
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 20px rgba(0,0,0,0.5));
        }

        .card-valen {
            background: rgba(0, 0, 0, 0.85); border: 2px solid var(--accent);
            border-radius: 25px; padding: 30px; max-width: 350px;
            margin: -40px auto 40px; text-align: center; backdrop-filter: blur(10px);
        }

        /* GRILLA DE 7 FACCIONES */
        .facciones-grid {
            display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 20px; padding: 0 8% 60px;
        }

        .f-card {
            background: rgba(255,255,255,0.05); border-radius: 20px; height: 180px;
            position: relative; overflow: hidden; border: 1px solid rgba(255,255,255,0.1);
            transition: 0.3s;
        }

        .f-card:hover { transform: translateY(-8px); border-color: rgba(255,255,255,0.3); }

        .f-info { height: 100%; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; }

        .f-jefe {
            position: absolute; bottom: -100%; width: 100%; height: 100%;
            display: flex; flex-direction: column; justify-content: center; align-items: center;
            transition: 0.4s ease-in-out; background: var(--cba-azul);
        }

        .f-card:hover .f-jefe { bottom: 0; }

        .discord-btn {
            background: #5865F2; color: white; padding: 15px 35px;
            border-radius: 12px; text-decoration: none; font-weight: 800;
            display: inline-block; margin-bottom: 40px; transition: 0.3s;
        }
        .discord-btn:hover { background: #4752c4; transform: scale(1.05); }

    </style>
</head>
<body>

<div class="hero-bg"></div>

<div class="sticker-v fernet-v">
    <i class="fas fa-wine-bottle fa-4x"></i>
    <div class="sticker-label">FERNET</div>
</div>
<div class="sticker-v coca-v">
    <i class="fas fa-glass-whiskey fa-4x"></i>
    <div class="sticker-label">COCA</div>
</div>

<header>
    <h1 class="titulo-cba">CÓRDOBA</h1>
    <h2 style="letter-spacing: 8px; font-weight: 200; margin: 0;">CAPITAL RP</h2>
    <p style="margin-top: 15px; opacity: 0.9;">164 Miembros | <i class="fas fa-music"></i> Sonando: Chingon - Desakata2</p>
</header>

<div class="card-valen">
    <i class="fas fa-crown" style="color: var(--accent); font-size: 2.5rem;"></i>
    <h2 style="margin: 10px 0;">VALEN</h2>
    <p style="color: var(--accent); font-weight: bold; margin: 0;">FUNDADOR & DIRECTOR</p>
    <p style="color: #2ecc71; font-size: 0.9rem; margin-top: 10px;"><i class="fas fa-circle"></i> STAFF ACTIVO</p>
</div>

<div style="text-align: center;">
    <a href="#" class="discord-btn"><i class="fab fa-discord"></i> ENTRAR AL DISCORD</a>
</div>

<div class="facciones-grid">
    <div class="f-card" style="border-bottom: 5px solid #0056b3;">
        <div class="f-info"><i class="fas fa-shield-halved fa-2x"></i><h3>Policía de Córdoba</h3></div>
        <div class="f-jefe" style="background: #0056b3;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #002244;">
        <div class="f-info"><i class="fas fa-building-shield fa-2x"></i><h3>Policía Federal</h3></div>
        <div class="f-jefe" style="background: #002244;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #ff6600;">
        <div class="f-info"><i class="fas fa-anchor fa-2x"></i><h3>Prefectura</h3></div>
        <div class="f-jefe" style="background: #ff6600;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #d32f2f;">
        <div class="f-info"><i class="fas fa-fire fa-2x"></i><h3>Bomberos</h3></div>
        <div class="f-jefe" style="background: #d32f2f;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #28a745;">
        <div class="f-info"><i class="fas fa-ambulance fa-2x"></i><h3>107 Cordobés</h3></div>
        <div class="f-jefe" style="background: #28a745;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #f1c40f;">
        <div class="f-info"><i class="fas fa-car-side fa-2x" style="color: #f1c40f;"></i><h3>Seguridad Vial</h3></div>
        <div class="f-jefe" style="background: #f1c40f; color: black;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>

    <div class="f-card" style="border-bottom: 5px solid #7f8c8d;">
        <div class="f-info"><i class="fas fa-user-shield fa-2x"></i><h3>Guardia Local</h3></div>
        <div class="f-jefe" style="background: #7f8c8d;"><p>JEFE DE FACCIÓN</p><h3>[Pendiente]</h3></div>
    </div>
</div>

<audio id="player" loop>
    <source src="musica.mp3" type="audio/mpeg">
</audio>

<script>
    const audio = document.getElementById("player");
    audio.volume = 0.15; // Volumen bajo para que sea agradable

    // El navegador necesita una interacción para dejar reproducir sonido
    document.addEventListener('click', () => {
        audio.play();
    }, { once: true });
</script>

</body>
</html>
