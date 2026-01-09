<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Curso de Verão GRÁTIS - Inglês Descomplicado</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;900&family=Fredoka:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-pink: #E91E8C;
            --primary-yellow: #FFD700;
            --primary-blue: #00A3E0;
            --primary-orange: #FF6B35;
            --bg-gradient: linear-gradient(135deg, #FF6B35 0%, #E91E8C 25%, #00A3E0 50%, #FFD700 75%, #FF6B35 100%);
            --text-dark: #2D2D2D;
            --text-light: #FFFFFF;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
            background: #FFF8E7;
            position: relative;
        }

        /* Animated Background */
        .animated-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: var(--bg-gradient);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .wave-decoration {
            position: absolute;
            width: 100%;
            height: 200px;
            top: 0;
            left: 0;
            overflow: hidden;
        }

        .wave {
            position: absolute;
            width: 200%;
            height: 100%;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120"><path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" fill="%23ffffff" opacity="0.3"/></svg>') repeat-x;
            animation: wave 20s linear infinite;
        }

        .wave:nth-child(2) {
            animation: wave 15s linear infinite reverse;
            opacity: 0.5;
        }

        @keyframes wave {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 1;
        }

        /* Header */
        header {
            text-align: center;
            padding: 60px 20px 40px;
            position: relative;
        }

        .badge {
            display: inline-block;
            background: var(--primary-pink);
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            font-family: 'Fredoka', sans-serif;
            font-weight: 700;
            font-size: 1.2rem;
            transform: rotate(-2deg);
            box-shadow: 0 8px 20px rgba(233, 30, 140, 0.4);
            animation: bounce 2s ease-in-out infinite;
            margin-bottom: 20px;
        }

        @keyframes bounce {
            0%, 100% { transform: rotate(-2deg) translateY(0); }
            50% { transform: rotate(-2deg) translateY(-10px); }
        }

        h1 {
            font-family: 'Fredoka', sans-serif;
            font-size: 4rem;
            font-weight: 900;
            color: white;
            text-shadow: 4px 4px 0 rgba(0, 0, 0, 0.2);
            line-height: 1.1;
            margin: 20px 0;
            animation: slideInDown 0.8s ease-out;
        }

        @keyframes slideInDown {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .highlight-yellow {
            color: var(--primary-yellow);
            display: block;
            font-size: 5rem;
            text-shadow: 
                3px 3px 0 var(--primary-pink),
                6px 6px 0 rgba(0, 0, 0, 0.2);
        }

        .subtitle {
            font-size: 1.8rem;
            color: white;
            font-weight: 600;
            margin: 20px 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            animation: slideInUp 0.8s ease-out 0.2s backwards;
        }

        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .emoji-large {
            font-size: 3rem;
            display: inline-block;
            animation: rotate 3s ease-in-out infinite;
        }

        @keyframes rotate {
            0%, 100% { transform: rotate(-10deg); }
            50% { transform: rotate(10deg); }
        }

        /* Main Content */
        .content-wrapper {
            background: white;
            border-radius: 40px;
            padding: 60px 40px;
            margin: 40px 0;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
            position: relative;
            overflow: hidden;
            animation: fadeInScale 0.8s ease-out 0.4s backwards;
        }

        @keyframes fadeInScale {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        .content-wrapper::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(255, 215, 0, 0.1) 0%, transparent 70%);
            animation: float 8s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            50% { transform: translate(50px, 50px) rotate(180deg); }
        }

        .info-section {
            margin: 40px 0;
            position: relative;
            z-index: 1;
        }

        h2 {
            font-family: 'Fredoka', sans-serif;
            font-size: 2.5rem;
            color: var(--primary-pink);
            margin-bottom: 30px;
            text-align: center;
            position: relative;
        }

        h2::after {
            content: '';
            display: block;
            width: 100px;
            height: 5px;
            background: var(--primary-yellow);
            margin: 15px auto 0;
            border-radius: 10px;
        }

        .details-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin: 40px 0;
        }

        .detail-card {
            background: linear-gradient(135deg, #FF6B35 0%, #E91E8C 100%);
            padding: 30px;
            border-radius: 25px;
            color: white;
            box-shadow: 0 10px 30px rgba(233, 30, 140, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .detail-card:hover {
            transform: translateY(-10px) rotate(2deg);
            box-shadow: 0 15px 40px rgba(233, 30, 140, 0.5);
        }

        .detail-icon {
            font-size: 3rem;
            margin-bottom: 15px;
            display: block;
        }

        .detail-card h3 {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 10px;
        }

        .detail-card p {
            font-size: 1.1rem;
            line-height: 1.6;
        }

        /* Form Section */
        .form-section {
            background: linear-gradient(135deg, #00A3E0 0%, #0077B6 100%);
            padding: 50px;
            border-radius: 30px;
            margin: 50px 0;
            box-shadow: 0 15px 40px rgba(0, 163, 224, 0.3);
        }

        .form-section h2 {
            color: white;
        }

        .form-section h2::after {
            background: white;
        }

        .form-group {
            margin-bottom: 25px;
        }

        label {
            display: block;
            font-weight: 600;
            font-size: 1.1rem;
            color: white;
            margin-bottom: 10px;
        }

        input[type="text"],
        input[type="tel"] {
            width: 100%;
            padding: 18px 25px;
            border: none;
            border-radius: 15px;
            font-size: 1.1rem;
            font-family: 'Poppins', sans-serif;
            background: white;
            box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }

        input[type="text"]:focus,
        input[type="tel"]:focus {
            outline: none;
            box-shadow: 0 0 0 4px rgba(255, 255, 255, 0.5);
            transform: translateY(-2px);
        }

        .checkbox-group {
            background: rgba(255, 255, 255, 0.15);
            padding: 25px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .checkbox-item {
            margin: 15px 0;
            position: relative;
        }

        .checkbox-item input[type="checkbox"] {
            position: absolute;
            opacity: 0;
            cursor: pointer;
        }

        .checkbox-label {
            display: flex;
            align-items: center;
            cursor: pointer;
            font-size: 1.1rem;
            padding: 15px 20px;
            background: white;
            border-radius: 12px;
            transition: all 0.3s ease;
            position: relative;
            padding-left: 60px;
        }

        .checkbox-label:hover {
            transform: translateX(5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .checkbox-label::before {
            content: '';
            position: absolute;
            left: 20px;
            width: 25px;
            height: 25px;
            border: 3px solid var(--primary-blue);
            border-radius: 6px;
            transition: all 0.3s ease;
        }

        .checkbox-item input[type="checkbox"]:checked + .checkbox-label {
            background: var(--primary-yellow);
            color: var(--text-dark);
            font-weight: 600;
        }

        .checkbox-item input[type="checkbox"]:checked + .checkbox-label::before {
            background: var(--primary-pink);
            border-color: var(--primary-pink);
        }

        .checkbox-item input[type="checkbox"]:checked + .checkbox-label::after {
            content: '✓';
            position: absolute;
            left: 24px;
            color: white;
            font-size: 1.2rem;
            font-weight: bold;
        }

        .submit-btn {
            background: linear-gradient(135deg, #FFD700 0%, #FFA500 100%);
            color: var(--text-dark);
            border: none;
            padding: 25px 60px;
            font-size: 1.5rem;
            font-weight: 700;
            font-family: 'Fredoka', sans-serif;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 10px 30px rgba(255, 165, 0, 0.4);
            transition: all 0.3s ease;
            display: block;
            margin: 40px auto 0;
            text-transform: uppercase;
            position: relative;
            overflow: hidden;
        }

        .submit-btn::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.5);
            transform: translate(-50%, -50%);
            transition: width 0.6s ease, height 0.6s ease;
        }

        .submit-btn:hover {
            transform: scale(1.1) rotate(-2deg);
            box-shadow: 0 15px 40px rgba(255, 165, 0, 0.6);
        }

        .submit-btn:hover::before {
            width: 300px;
            height: 300px;
        }

        .submit-btn:active {
            transform: scale(1.05) rotate(-2deg);
        }

        /* Success Message */
        .success-message {
            background: linear-gradient(135deg, #4CAF50 0%, #45B649 100%);
            color: white;
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            font-size: 1.3rem;
            font-weight: 600;
            margin-top: 30px;
            display: none;
            animation: slideInUp 0.5s ease-out;
            box-shadow: 0 10px 30px rgba(76, 175, 80, 0.4);
        }

        .success-message.show {
            display: block;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 20px;
            color: white;
            font-size: 1.1rem;
        }

        .whatsapp-info {
            background: #25D366;
            display: inline-block;
            padding: 20px 40px;
            border-radius: 50px;
            font-weight: 700;
            margin: 20px 0;
            box-shadow: 0 8px 25px rgba(37, 211, 102, 0.4);
            text-decoration: none;
            color: white;
            transition: all 0.3s ease;
        }

        .whatsapp-info:hover {
            transform: scale(1.1);
            box-shadow: 0 12px 35px rgba(37, 211, 102, 0.6);
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }

            .highlight-yellow {
                font-size: 3rem;
            }

            .subtitle {
                font-size: 1.3rem;
            }

            .content-wrapper {
                padding: 40px 25px;
                border-radius: 25px;
            }

            .form-section {
                padding: 30px 20px;
            }

            .details-grid {
                grid-template-columns: 1fr;
            }

            .submit-btn {
                font-size: 1.2rem;
                padding: 20px 40px;
            }
        }

        /* Floating decorative elements */
        .floating-emoji {
            position: fixed;
            font-size: 3rem;
            opacity: 0.3;
            animation: floatAround 20s ease-in-out infinite;
            z-index: 0;
            pointer-events: none;
        }

        @keyframes floatAround {
            0%, 100% {
                transform: translate(0, 0) rotate(0deg);
            }
            25% {
                transform: translate(100px, -100px) rotate(90deg);
            }
            50% {
                transform: translate(-50px, -50px) rotate(180deg);
            }
            75% {
                transform: translate(-100px, 100px) rotate(270deg);
            }
        }

        .floating-emoji:nth-child(1) { top: 10%; left: 10%; animation-delay: 0s; }
        .floating-emoji:nth-child(2) { top: 20%; right: 15%; animation-delay: 2s; }
        .floating-emoji:nth-child(3) { bottom: 20%; left: 15%; animation-delay: 4s; }
        .floating-emoji:nth-child(4) { bottom: 30%; right: 10%; animation-delay: 6s; }
    </style>
</head>
<body>
    <div class="animated-bg"></div>
    
    <!-- Floating decorative emojis -->
    <div class="floating-emoji">🎵</div>
    <div class="floating-emoji">🎧</div>
    <div class="floating-emoji">🎬</div>
    <div class="floating-emoji">📱</div>

    <div class="container">
        <header>
            <div class="badge">🎓 CURSO DE VERÃO</div>
            <h1>
                <span class="highlight-yellow">GRÁTIS</span>
                INGLÊS DESCOMPLICADO
            </h1>
            <p class="subtitle">
                Aprenda com as músicas e séries<br>
                que você <strong>JÁ AMA</strong> <span class="emoji-large">❤️</span>
            </p>
        </header>

        <div class="content-wrapper">
            <div class="info-section">
                <h2>🔥 NADA DE DECOREBA CHATA!</h2>
                <p style="text-align: center; font-size: 1.3rem; color: var(--text-dark); margin: 20px 0;">
                    Aqui você aprende de verdade!
                </p>

                <div class="details-grid">
                    <div class="detail-card">
                        <span class="detail-icon">📅</span>
                        <h3>4 Encontros Incríveis</h3>
                        <p>Quintas: 15/01, 22/01, 29/01 e 05/02</p>
                    </div>

                    <div class="detail-card">
                        <span class="detail-icon">⏰</span>
                        <h3>Horário Perfeito</h3>
                        <p>10h às 12h - Aproveite sua manhã!</p>
                    </div>

                    <div class="detail-card">
                        <span class="detail-icon">📍</span>
                        <h3>Local</h3>
                        <p>Auditório da Microlins<br>Av. Ver. Edenites da Silva Viana, 86 - Altos</p>
                    </div>
                </div>
            </div>

            <div class="form-section">
                <h2>✨ INSCREVA-SE GRÁTIS!</h2>
                
                <form id="registrationForm">
                    <div class="form-group">
                        <label for="fullName">Nome Completo *</label>
                        <input type="text" id="fullName" name="fullName" required placeholder="Seu nome completo">
                    </div>

                    <div class="form-group">
                        <label for="phone">Telefone do Responsável *</label>
                        <input type="tel" id="phone" name="phone" required placeholder="(00) 00000-0000">
                    </div>

                    <div class="form-group">
                        <label>Áreas de Interesse (marque quantas quiser):</label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" id="ingles" name="areas" value="Inglês">
                                <label for="ingles" class="checkbox-label">🇬🇧 Inglês</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="games" name="areas" value="Games">
                                <label for="games" class="checkbox-label">🎮 Games</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="ia" name="areas" value="Inteligência Artificial">
                                <label for="ia" class="checkbox-label">🤖 Inteligência Artificial</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="computadores" name="areas" value="Montagem e Manutenção de Computadores">
                                <label for="computadores" class="checkbox-label">💻 Montagem e Manutenção de Computadores</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="apps" name="areas" value="Criação de Aplicativos">
                                <label for="apps" class="checkbox-label">📱 Criação de Aplicativos</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" id="videos" name="areas" value="Edição de Vídeos">
                                <label for="videos" class="checkbox-label">?# curso-verao-ingles
Inscritos para curso de verão gratuito
