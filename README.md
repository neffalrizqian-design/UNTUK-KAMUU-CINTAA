<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>🎂 HBD Sayangku ❤️</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&family=Nunito:wght@400;600;700;800;900&family=Dancing+Script:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }

        html, body {
            min-height: 100vh;
            width: 100%;
            overflow-x: hidden;
        }

        body {
            background: linear-gradient(145deg, #fce4ec, #f8bbd0, #fce4ec);
            font-family: 'Nunito', sans-serif;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            padding: 1rem;
            position: relative;
            min-height: 100vh;
        }

        .bg-emoji {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            overflow: hidden;
            opacity: 0.5;
        }
        .bg-emoji span {
            position: absolute;
            animation: fallEmoji 8s linear infinite;
            font-size: 2rem;
        }
        @keyframes fallEmoji {
            0% { transform: translateY(-100px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(110vh) rotate(720deg); opacity: 0; }
        }

        .card {
            position: relative;
            z-index: 10;
            max-width: 560px;
            width: 100%;
            background: rgba(255, 248, 250, 0.88);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border-radius: 48px;
            padding: 1.8rem 1.5rem 2rem;
            box-shadow: 0 30px 60px rgba(180, 60, 100, 0.2);
            border: 1px solid rgba(255, 220, 235, 0.6);
            text-align: center;
            margin: 0.5rem auto;
            max-height: 98vh;
            overflow-y: auto;
        }
        .card::-webkit-scrollbar { width: 4px; }
        .card::-webkit-scrollbar-thumb { background: #ff4d7a; border-radius: 10px; }

        .page { display: none; animation: fadePage 0.6s cubic-bezier(0.34, 1.56, 0.64, 1); }
        .page.active { display: block; }
        @keyframes fadePage {
            0% { opacity: 0; transform: scale(0.92) translateY(20px); }
            100% { opacity: 1; transform: scale(1) translateY(0); }
        }

        .title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.4rem;
            color: #b31b4b;
            letter-spacing: 1px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            animation: stretchText 2s ease-in-out infinite alternate;
        }
        @keyframes stretchText {
            0% { transform: scale(1) rotate(-1deg); letter-spacing: 1px; }
            100% { transform: scale(1.05) rotate(1deg); letter-spacing: 3px; }
        }
        .title i { color: #d43f6b; font-size: 2rem; }

        .sub {
            font-weight: 700;
            font-size: 1rem;
            color: #a53f5f;
            background: rgba(255, 200, 215, 0.3);
            display: inline-block;
            padding: 0.3rem 1.8rem;
            border-radius: 60px;
            margin: 0.3rem 0 1.2rem;
        }

        .btn-slime {
            background: linear-gradient(135deg, #ff6b9d, #ff4d7a, #e63e6b);
            border: none;
            padding: 0.8rem 2.4rem;
            border-radius: 100px;
            color: white;
            font-weight: 800;
            font-size: 1.4rem;
            font-family: 'Fredoka One', cursive;
            display: inline-flex;
            align-items: center;
            gap: 12px;
            box-shadow: 0 10px 30px rgba(230, 50, 90, 0.5), inset 0 -4px 0 rgba(0,0,0,0.1);
            cursor: pointer;
            transition: all 0.15s cubic-bezier(0.34, 1.56, 0.64, 1);
            border: 2px solid rgba(255, 255, 255, 0.3);
            min-width: 140px;
            justify-content: center;
            position: relative;
            animation: slimeIdle 2s ease-in-out infinite;
        }
        @keyframes slimeIdle {
            0%, 100% { transform: scale(1) rotate(0deg); }
            50% { transform: scale(1.03) rotate(1deg); }
        }
        .btn-slime:hover {
            transform: scale(1.2) rotate(-3deg);
            box-shadow: 0 18px 40px rgba(230, 50, 90, 0.6);
            animation: none;
        }
        .btn-slime:active {
            transform: scale(0.85) rotate(5deg);
            transition-duration: 0.05s;
            box-shadow: 0 5px 15px rgba(230, 50, 90, 0.4);
        }
        .btn-slime i { font-size: 1.4rem; }

        /* AMPLOP */
        .envelope-container {
            position: relative;
            margin: 1rem auto;
            cursor: pointer;
            animation: floatEnvelope 3s ease-in-out infinite;
            display: inline-block;
        }
        @keyframes floatEnvelope {
            0%, 100% { transform: translateY(0px) rotate(-2deg); }
            50% { transform: translateY(-15px) rotate(2deg); }
        }
        .envelope {
            position: relative;
            width: 300px;
            height: 190px;
            background: linear-gradient(145deg, #ffd6e0, #ffb6c9);
            border-radius: 16px 16px 10px 10px;
            box-shadow: 0 15px 45px rgba(180, 60, 100, 0.35), inset 0 -4px 0 rgba(200, 80, 120, 0.2);
            border: 3px solid #ff8aaa;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            overflow: hidden;
        }
        .envelope::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: repeating-linear-gradient(
                45deg,
                transparent,
                transparent 10px,
                rgba(255, 255, 255, 0.05) 10px,
                rgba(255, 255, 255, 0.05) 20px
            );
            pointer-events: none;
        }
        .envelope .envelope-icon {
            font-size: 4.5rem;
            z-index: 2;
            position: relative;
            color: #ff4d7a;
            filter: drop-shadow(0 4px 15px rgba(255, 77, 122, 0.3));
            animation: pulseEnvelope 2s ease-in-out infinite;
        }
        @keyframes pulseEnvelope {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }
        .envelope .heart-deco {
            position: absolute;
            font-size: 1.6rem;
            color: #ff4d7a;
            animation: pulseDeco 1.5s ease-in-out infinite;
            filter: drop-shadow(0 0 8px rgba(255, 77, 122, 0.3));
        }
        .envelope .heart-deco:nth-child(1) { top: 12px; left: 18px; }
        .envelope .heart-deco:nth-child(2) { top: 12px; right: 18px; }
        .envelope .heart-deco:nth-child(3) { bottom: 12px; left: 18px; }
        .envelope .heart-deco:nth-child(4) { bottom: 12px; right: 18px; }
        .envelope .star-deco {
            position: absolute;
            font-size: 1.4rem;
            color: #ffd700;
            animation: sparkle 1.8s ease-in-out infinite;
            filter: drop-shadow(0 0 8px rgba(255, 215, 0, 0.3));
        }
        .envelope .star-deco:nth-child(5) { top: 50%; left: 10px; animation-delay: 0.2s; }
        .envelope .star-deco:nth-child(6) { top: 50%; right: 10px; animation-delay: 0.7s; }
        .envelope .envelope-line {
            position: absolute;
            top: 50%;
            left: 20px;
            right: 20px;
            height: 2px;
            background: rgba(255, 77, 122, 0.2);
            border-top: 2px dashed rgba(255, 77, 122, 0.3);
        }
        @keyframes pulseDeco {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.3); }
        }
        @keyframes sparkle {
            0%, 100% { opacity: 0.5; transform: scale(0.8) rotate(0deg); }
            50% { opacity: 1; transform: scale(1.2) rotate(180deg); }
        }

        /* ISI AMPLOP */
        .envelope-content {
            display: none;
            animation: fadeContent 0.8s cubic-bezier(0.34, 1.56, 0.64, 1);
            margin-top: 1rem;
        }
        .envelope-content.open {
            display: block;
        }
        @keyframes fadeContent {
            0% { opacity: 0; transform: scale(0.8) translateY(20px); }
            100% { opacity: 1; transform: scale(1) translateY(0); }
        }

        .photo-frame {
            position: relative;
            display: inline-block;
            padding: 10px;
            background: linear-gradient(135deg, #ff6b9d, #ff4d7a);
            border-radius: 30px;
            box-shadow: 0 8px 30px rgba(255, 77, 122, 0.3);
            margin: 0.5rem 0;
            border: 3px solid white;
        }
        .photo-frame::before {
            content: '❤️';
            position: absolute;
            top: -15px;
            left: -15px;
            font-size: 2rem;
            animation: pulseDeco 1.5s ease-in-out infinite;
        }
        .photo-frame::after {
            content: '❤️';
            position: absolute;
            bottom: -15px;
            right: -15px;
            font-size: 2rem;
            animation: pulseDeco 1.5s ease-in-out infinite 0.5s;
        }
        .photo-frame img {
            width: 200px;
            height: 200px;
            object-fit: cover;
            border-radius: 20px;
            display: block;
            border: 3px solid white;
        }

        .letter-text {
            font-family: 'Dancing Script', cursive;
            font-size: 1.3rem;
            color: #4a1a2a;
            line-height: 2;
            background: rgba(255, 248, 250, 0.8);
            padding: 1.2rem;
            border-radius: 30px;
            border: 1px solid rgba(255, 200, 215, 0.4);
            margin: 0.8rem 0;
            text-align: left;
            position: relative;
            backdrop-filter: blur(4px);
        }
        .letter-text .close-btn {
            position: absolute;
            top: 8px;
            right: 12px;
            font-size: 0.9rem;
            color: #ff4d7a;
            cursor: pointer;
            background: rgba(255, 200, 215, 0.3);
            padding: 2px 12px;
            border-radius: 20px;
            border: none;
            font-family: 'Fredoka One', cursive;
            transition: all 0.3s ease;
        }
        .letter-text .close-btn:hover {
            transform: scale(1.1);
            background: rgba(255, 77, 122, 0.3);
        }

        .music-player {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: linear-gradient(145deg, #2a2a3a, #1a1a2a);
            padding: 10px 20px;
            border-radius: 60px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.3), inset 0 2px 0 rgba(255,255,255,0.1);
            border: 1px solid #444;
            margin: 0.5rem 0;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .music-player:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 35px rgba(0,0,0,0.4);
        }
        .music-player .disc {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: radial-gradient(circle at 30% 30%, #888, #333);
            border: 2px solid #555;
            animation: spinDisc 3s linear infinite paused;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            color: #ff4d7a;
        }
        .music-player.playing .disc {
            animation-play-state: running;
        }
        @keyframes spinDisc {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        .music-player .label {
            font-family: 'Fredoka One', cursive;
            color: #ddd;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }
        .music-player .label i { color: #ff4d7a; margin-right: 5px; }

        .quiz-question {
            font-family: 'Fredoka One', cursive;
            font-size: 1.3rem;
            color: #b31b4b;
            margin: 0.8rem 0;
        }
        .quiz-options {
            display: flex;
            flex-direction: column;
            gap: 0.6rem;
            margin: 0.8rem 0;
        }
        .quiz-option {
            background: rgba(255, 255, 255, 0.5);
            padding: 0.8rem 1.2rem;
            border-radius: 30px;
            border: 2px solid rgba(255, 200, 215, 0.4);
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 700;
            color: #4a1a2a;
        }
        .quiz-option:hover {
            transform: scale(1.03);
            border-color: #ff4d7a;
            background: rgba(255, 200, 215, 0.3);
        }
        .quiz-option.correct {
            border-color: #4caf50;
            background: rgba(76, 175, 80, 0.2);
        }
        .quiz-option.wrong {
            border-color: #f44336;
            background: rgba(244, 67, 54, 0.2);
        }
        .quiz-result {
            font-family: 'Dancing Script', cursive;
            font-size: 1.5rem;
            color: #b31b4b;
            margin: 0.8rem 0;
        }

        .btn-small {
            background: linear-gradient(135deg, #ff6b9d, #ff4d7a);
            border: none;
            padding: 0.4rem 1.2rem;
            border-radius: 60px;
            color: white;
            font-weight: 700;
            font-size: 0.9rem;
            font-family: 'Fredoka One', cursive;
            cursor: pointer;
            transition: all 0.2s cubic-bezier(0.34, 1.56, 0.64, 1);
            box-shadow: 0 4px 15px rgba(230, 50, 90, 0.3);
        }
        .btn-small:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 25px rgba(230, 50, 90, 0.4);
        }

        /* ANIMASI LEDAKAN */
        .explode-particle {
            position: fixed;
            pointer-events: none;
            z-index: 45;
            font-size: 2.5rem;
            animation: explodeParticle 3.5s ease-out forwards;
            opacity: 0;
        }
        @keyframes explodeParticle {
            0% { opacity: 0; transform: translate(0, 0) scale(0.3) rotate(0deg); }
            15% { opacity: 1; transform: translate(var(--tx), var(--ty)) scale(1.5) rotate(45deg); }
            60% { opacity: 1; }
            100% { opacity: 0; transform: translate(var(--tx2), var(--ty2)) scale(0.2) rotate(360deg); }
        }

        @media (max-width: 480px) {
            .card { padding: 1rem 0.8rem; max-height: 98vh; }
            .envelope { width: 220px; height: 150px; }
            .photo-frame img { width: 140px; height: 140px; }
            .title { font-size: 1.8rem; }
            .btn-slime { font-size: 1.1rem; padding: 0.6rem 1.6rem; min-width: 100px; }
            .letter-text { font-size: 1.1rem; }
            .envelope .envelope-icon { font-size: 3.5rem; }
            .explode-particle { font-size: 2rem; }
        }
        @media (max-width: 380px) {
            .card { padding: 0.8rem 0.5rem; }
            .envelope { width: 180px; height: 130px; }
            .photo-frame img { width: 110px; height: 110px; }
            .title { font-size: 1.4rem; }
            .btn-slime { font-size: 0.9rem; padding: 0.5rem 1.2rem; min-width: 80px; }
            .letter-text { font-size: 0.95rem; padding: 0.8rem; }
            .envelope .envelope-icon { font-size: 2.8rem; }
            .envelope .heart-deco { font-size: 1.2rem; }
            .envelope .star-deco { font-size: 1rem; }
            .explode-particle { font-size: 1.5rem; }
        }
    </style>
</head>
<body>

    <!-- Background Emoji Jatuhan -->
    <div class="bg-emoji" id="bgEmoji"></div>

    <!-- Card Utama -->
    <div class="card">

        <!-- HALAMAN 1: Pembuka -->
        <div class="page active" id="page1">
            <div class="title">
                <i class="fas fa-heart"></i>
                HAI MANISS
                <i class="fas fa-heart"></i>
            </div>
            <div class="sub">
                <i class="fas fa-arrow-right"></i> TOLONG DI BACA YA <i class="fas fa-arrow-left"></i>
            </div>
            <div style="margin: 2rem 0;">
                <button class="btn-slime" id="btnNext1">
                    <i class="fas fa-arrow-right"></i> SELANJUTNYA
                </button>
            </div>
        </div>

        <!-- HALAMAN 2: Amplop -->
        <div class="page" id="page2">
            <div class="title">
                <i class="fas fa-gift"></i>
                UNTUK MU
                <i class="fas fa-heart"></i>
            </div>
            <div class="sub" style="animation: stretchText 2s ease-in-out infinite alternate;">
                HARAP DI BUKA YA CANTIK 😘🥰
            </div>

            <!-- Amplop Melayang -->
            <div class="envelope-container" id="envelopeContainer">
                <div class="envelope" id="envelope">
                    <span class="heart-deco">❤️</span>
                    <span class="heart-deco">💖</span>
                    <span class="heart-deco">💗</span>
                    <span class="heart-deco">💕</span>
                    <span class="star-deco">⭐</span>
                    <span class="star-deco">✨</span>
                    <div class="envelope-line"></div>
                    <span class="envelope-icon">💌</span>
                </div>
            </div>

            <!-- ISI AMPLOP -->
            <div class="envelope-content" id="envelopeContent">
                <div class="photo-frame">
                    <img src="kamu4.jpg" alt="Foto Kamu" id="fotoAmplop">
                </div>
                <div class="letter-text" id="letterText">
                    <button class="close-btn" id="closeLetter">✕ TUTUP</button>
                    <div id="letterContent">
                        HBBBDDD SAYANGGG 🎂❤️<br>
                        SEMOGAAA KAMU PANJANG UMUR, SEHAT SELALU, DI MUDAHKAN REJEKINYA, BERBAKTI KEPADA ORANG TUA, MAKIN PINTAR, SUKSES DUNIAA AKHIRATT.<br>
                        DAN HUBUNGAN KITAA LANGGENGG TERUSS YAA SAYANGG CANTIK CINTAAA KUU KASIHH KUU 😘🥰🥰<br>
                        HBBDDD POKONYA CINTAAA. 💖🎉
                        F4T4N 4You
                    </div>
                    <div id="letterClosed" style="display:none; color:#b31b4b; font-size:1.2rem;">
                        💌 Surat sudah ditutup 💌
                    </div>
                </div>
            </div>

            <div style="margin: 0.5rem 0;">
                <button class="btn-slime" id="btnNext2" style="font-size:1.1rem; padding:0.6rem 1.8rem;">
                    <i class="fas fa-arrow-right"></i> SELANJUTNYA
                </button>
            </div>
        </div>

        <!-- HALAMAN 3: Kuis & Musik -->
        <div class="page" id="page3">
            <div class="title">
                <i class="fas fa-gamepad"></i>
                KUIZZ CINTA
                <i class="fas fa-heart"></i>
            </div>
            <div class="sub">
                <i class="fas fa-question-circle"></i> TEBAK² DRAMATIS <i class="fas fa-question-circle"></i>
            </div>

            <div class="photo-frame" style="padding:6px; border-radius:20px;">
                <img src="kamu3.jpg" alt="Foto Kamu" id="fotoKuis" style="width:120px; height:120px; border-radius:12px;">
            </div>

            <div class="music-player" id="musicPlayer">
                <div class="disc">💿</div>
                <span class="label"><i class="fas fa-music"></i> Putar Lagu</span>
            </div>

            <div id="quizContainer">
                <div class="quiz-question" id="quizQuestion">Apa yang paling kamu suka dari aku?</div>
                <div class="quiz-options" id="quizOptions">
                    <div class="quiz-option" data-correct="true">❤️ Kebaikan hatimu</div>
                    <div class="quiz-option" data-correct="false">😅 Kekocakanmu</div>
                    <div class="quiz-option" data-correct="false">😏 Kejahilanmu</div>
                    <div class="quiz-option" data-correct="false">🤔 Semua salah</div>
                </div>
                <div class="quiz-result" id="quizResult"></div>
                <div style="margin-top:0.5rem;">
                    <button class="btn-small" id="btnNextQuiz">Selanjutnya →</button>
                </div>
            </div>

            <div style="margin: 0.5rem 0;">
                <button class="btn-small" id="btnFinish" style="font-size:1rem; padding:0.5rem 1.5rem;">🎉 Selesai</button>
            </div>
        </div>

    </div>

    <audio id="bgMusic" loop style="display:none;">
        <source src="kamu7.mp3" type="audio/mp3">
    </audio>

    <script>
        (function() {
            // ===== BACKGROUND EMOJI =====
            const bgEmoji = document.getElementById('bgEmoji');
            const emojis = ['❤️', '💖', '💗', '💘', '💝', '✨', '🎂', '🎉', '🎁', '💕', '💋', '🥰', '😘', '🌹', '🌸'];
            for (let i = 0; i < 35; i++) {
                const span = document.createElement('span');
                span.textContent = emojis[Math.floor(Math.random() * emojis.length)];
                span.style.left = Math.random() * 100 + '%';
                span.style.animationDuration = 6 + Math.random() * 8 + 's';
                span.style.animationDelay = Math.random() * 10 + 's';
                span.style.fontSize = 1.2 + Math.random() * 2.2 + 'rem';
                span.style.opacity = 0.2 + Math.random() * 0.4;
                bgEmoji.appendChild(span);
            }

            // ===== DOM =====
            const pages = {
                page1: document.getElementById('page1'),
                page2: document.getElementById('page2'),
                page3: document.getElementById('page3')
            };

            const btnNext1 = document.getElementById('btnNext1');
            const btnNext2 = document.getElementById('btnNext2');
            const btnNextQuiz = document.getElementById('btnNextQuiz');
            const btnFinish = document.getElementById('btnFinish');
            const envelope = document.getElementById('envelope');
            const envelopeContent = document.getElementById('envelopeContent');
            const closeLetter = document.getElementById('closeLetter');
            const letterContent = document.getElementById('letterContent');
            const letterClosed = document.getElementById('letterClosed');
            const musicPlayer = document.getElementById('musicPlayer');
            const bgMusic = document.getElementById('bgMusic');

            let isEnvelopeOpen = false;
            let musicPlaying = false;

            // ===== STYLE UNTUK ANIMASI =====
            if (!document.getElementById('explodeStyle')) {
                const style = document.createElement('style');
                style.id = 'explodeStyle';
                style.textContent = `
                    @keyframes bubbleUp {
                        0% { opacity:0; transform: translateY(0) scale(0.3) rotate(0deg); }
                        15% { opacity:1; transform: translateY(-30px) scale(1.3) rotate(10deg); }
                        80% { opacity:1; }
                        100% { opacity:0; transform: translateY(-150vh) scale(0.5) rotate(720deg); }
                    }
                    @keyframes love3dSpin {
                        0% { transform: translate(-50%,-50%) scale(0.2) rotateY(0deg); opacity:0; }
                        15% { transform: translate(-50%,-50%) scale(1.5) rotateY(-180deg); opacity:1; }
                        30% { transform: translate(-50%,-50%) scale(2.0) rotateY(-360deg); opacity:1; }
                        50% { transform: translate(-50%,-50%) scale(3.0) rotateY(-540deg); opacity:1; }
                        70% { transform: translate(-50%,-50%) scale(4.0) rotateY(-720deg); opacity:1; }
                        85% { transform: translate(-50%,-50%) scale(5.0) rotateY(-900deg); opacity:1; }
                        100% { transform: translate(-50%,-50%) scale(0) rotateY(-1080deg); opacity:0; }
                    }
                `;
                document.head.appendChild(style);
            }

            function showPage(pageId) {
                Object.keys(pages).forEach(key => {
                    pages[key].classList.remove('active');
                    pages[key].style.display = 'none';
                });
                pages[pageId].style.display = 'block';
                setTimeout(() => pages[pageId].classList.add('active'), 50);
            }

            // ===== TOMBOL SELANJUTNYA 1 =====
            btnNext1.addEventListener('click', function() {
                const loveEmojis = ['❤️', '💖', '💗', '💘', '💝', '✨', '💕', '💋', '🥰', '😘', '🌹', '🎂', '🎉'];
                for (let i = 0; i < 40; i++) {
                    const el = document.createElement('div');
                    el.style.cssText = `
                        position: fixed; pointer-events: none; z-index: 50;
                        font-size: ${1.5 + Math.random() * 3}rem;
                        left: ${Math.random() * 90 + 5}%; top: ${Math.random() * 90 + 5}%;
                        animation: bubbleUp 2s ease-out forwards; opacity: 0;
                    `;
                    el.textContent = loveEmojis[Math.floor(Math.random() * loveEmojis.length)];
                    document.body.appendChild(el);
                    setTimeout(() => el.remove(), 2200);
                }
                this.style.transform = 'scale(0.9)';
                setTimeout(() => { this.style.transform = ''; }, 150);
                setTimeout(() => showPage('page2'), 400);
            });

            // ===== AMPLOP KLIK - DENGAN LEDAKAN LENGKAP =====
            envelope.addEventListener('click', function() {
                if (isEnvelopeOpen) return;
                isEnvelopeOpen = true;

                // 1. LOVE BESAR 3D BERPUTAR
                const loveEl = document.createElement('div');
                loveEl.style.cssText = `
                    position: fixed; top:50%; left:50%; transform:translate(-50%,-50%);
                    font-size: 10rem; z-index: 40; pointer-events: none;
                    animation: love3dSpin 2.8s ease-in-out forwards;
                    text-shadow: 0 0 60px rgba(255,50,100,0.8);
                `;
                loveEl.textContent = '❤️';
                document.body.appendChild(loveEl);

                // 2. LEDAKAN EMOJI KUE, LILIN, API, LOVE, BUNGA DLL
                setTimeout(() => {
                    const cakeEmojis = ['🎂', '🎉', '🎁', '❤️', '💖', '💗', '✨', '🌟', '🥳', '🎊', '🕯️', '🔥', '🎈', '🌸', '🌺', '💕', '💘', '💝', '💋', '🥰', '😘', '🌹'];
                    const centerX = window.innerWidth / 2;
                    const centerY = window.innerHeight / 2;
                    
                    for (let i = 0; i < 70; i++) {
                        const el = document.createElement('div');
                        el.className = 'explode-particle';
                        const angle = Math.random() * Math.PI * 2;
                        const dist = 80 + Math.random() * 500;
                        const tx = Math.cos(angle) * dist;
                        const ty = Math.sin(angle) * dist - 80;
                        const tx2 = Math.cos(angle) * (dist + 120 + Math.random() * 200);
                        const ty2 = Math.sin(angle) * (dist + 120 + Math.random() * 200) - 160;
                        
                        el.style.left = centerX + 'px';
                        el.style.top = centerY + 'px';
                        el.style.setProperty('--tx', tx + 'px');
                        el.style.setProperty('--ty', ty + 'px');
                        el.style.setProperty('--tx2', tx2 + 'px');
                        el.style.setProperty('--ty2', ty2 + 'px');
                        el.style.fontSize = (1.8 + Math.random() * 3.2) + 'rem';
                        el.style.animationDuration = (2.8 + Math.random() * 1.8) + 's';
                        el.style.animationDelay = (Math.random() * 0.6) + 's';
                        el.textContent = cakeEmojis[Math.floor(Math.random() * cakeEmojis.length)];
                        document.body.appendChild(el);
                        setTimeout(() => el.remove(), 4500);
                    }
                }, 1400);

                // 3. TAMPILKAN ISI AMPLOP
                setTimeout(() => {
                    envelopeContent.classList.add('open');
                    setTimeout(() => {
                        envelopeContent.scrollIntoView({ behavior: 'smooth', block: 'center' });
                    }, 300);
                }, 2200);

                setTimeout(() => loveEl.remove(), 3200);
                this.style.transform = 'scale(0.95)';
                setTimeout(() => { this.style.transform = ''; }, 200);
            });

            // ===== TUTUP SURAT =====
            closeLetter.addEventListener('click', function() {
                letterContent.style.display = 'none';
                letterClosed.style.display = 'block';
                this.style.transform = 'scale(0.9)';
                setTimeout(() => { this.style.transform = ''; }, 150);
            });

            // ===== TOMBOL SELANJUTNYA 2 =====
            btnNext2.addEventListener('click', function() {
                showPage('page3');
                this.style.transform = 'scale(0.9)';
                setTimeout(() => { this.style.transform = ''; }, 150);
            });

            // ===== MUSIC PLAYER =====
            musicPlayer.addEventListener('click', function() {
                if (musicPlaying) {
                    bgMusic.pause();
                    this.classList.remove('playing');
                    musicPlaying = false;
                    this.querySelector('.label').innerHTML = '<i class="fas fa-music"></i> Putar Lagu';
                } else {
                    bgMusic.volume = 1.0;
                    bgMusic.currentTime = 0;
                    bgMusic.play().then(() => {
                        this.classList.add('playing');
                        musicPlaying = true;
                        this.querySelector('.label').innerHTML = '<i class="fas fa-pause"></i> Putar Lagu';
                    }).catch(e => {
                        console.log('Audio play error:', e);
                        alert('File audio tidak ditemukan. Pastikan kamu7.mp3 ada di folder yang sama.');
                    });
                }
                this.style.transform = 'scale(0.95)';
                setTimeout(() => { this.style.transform = ''; }, 150);
            });

            // ===== KUIZ =====
            const quizData = [
                {
                    question: "Apa yang paling kamu suka dari aku?",
                    options: ["❤️ Kebaikan hatimu", "😅 Kekocakanmu", "😏 Kejahilanmu", "🤔 Semua salah"],
                    correct: 0
                },
                {
                    question: "Apa janji kita berdua?",
                    options: ["😅 Putus dalam 1 bulan", "❤️ Sampai tua bersama", "😏 Cuma main-main", "🤔 Gak tau"],
                    correct: 1
                },
                {
                    question: "Kapan kita pertama kali ketemu?",
                    options: ["😅 Di sekolah", "❤️ Di kafe", "😏 Di taman", "🤔 Lupa"],
                    correct: 1
                }
            ];

            let currentQuiz = 0;
            let quizAnswered = false;

            function loadQuiz(index) {
                if (index >= quizData.length) {
                    document.getElementById('quizContainer').style.display = 'none';
                    document.querySelector('.quiz-result').textContent = '🎉 SELESAI SEMUA! KAMU HEBAT! ❤️';
                    return;
                }
                const data = quizData[index];
                document.getElementById('quizQuestion').textContent = data.question;
                const options = document.getElementById('quizOptions');
                options.innerHTML = '';
                data.options.forEach((opt, i) => {
                    const div = document.createElement('div');
                    div.className = 'quiz-option';
                    div.textContent = opt;
                    div.dataset.correct = (i === data.correct) ? 'true' : 'false';
                    div.addEventListener('click', function() {
                        if (quizAnswered) return;
                        quizAnswered = true;
                        const isCorrect = this.dataset.correct === 'true';
                        this.classList.add(isCorrect ? 'correct' : 'wrong');
                        document.getElementById('quizResult').textContent = isCorrect ? 
                            '✅ Benar! Kamu hebat! ❤️' : '❌ Salah! Coba lagi nanti 😅';
                        if (isCorrect) {
                            for (let i = 0; i < 20; i++) {
                                const el = document.createElement('div');
                                el.style.cssText = `
                                    position: fixed; pointer-events: none; z-index: 50;
                                    font-size: ${1 + Math.random() * 2}rem;
                                    left: ${Math.random() * 90 + 5}%; top: ${Math.random() * 90 + 5}%;
                                    animation: bubbleUp 2s ease-out forwards; opacity: 0;
                                `;
                                el.textContent = ['❤️','💖','💗','✨','🥰'][Math.floor(Math.random()*5)];
                                document.body.appendChild(el);
                                setTimeout(() => el.remove(), 2200);
                            }
                        }
                        document.querySelectorAll('.quiz-option').forEach(o => o.style.pointerEvents = 'none');
                        setTimeout(() => {
                            if (index < quizData.length - 1) {
                                document.getElementById('btnNextQuiz').style.display = 'inline-block';
                            } else {
                                document.getElementById('btnNextQuiz').textContent = '🎉 Selesai!';
                                document.getElementById('btnNextQuiz').style.display = 'inline-block';
                            }
                        }, 800);
                    });
                    options.appendChild(div);
                });
                document.getElementById('btnNextQuiz').style.display = 'none';
                document.getElementById('quizResult').textContent = '';
                quizAnswered = false;
                document.querySelectorAll('.quiz-option').forEach(o => {
                    o.classList.remove('correct', 'wrong');
                    o.style.pointerEvents = 'auto';
                });
            }

            btnNextQuiz.addEventListener('click', function() {
                currentQuiz++;
                if (currentQuiz >= quizData.length) {
                    document.getElementById('quizContainer').style.display = 'none';
                    document.querySelector('.quiz-result').textContent = '🎉 SEMUA JAWABAN BENAR! KAMU LUAR BIASA! ❤️';
                    this.style.display = 'none';
                    return;
                }
                loadQuiz(currentQuiz);
                this.style.transform = 'scale(0.9)';
                setTimeout(() => { this.style.transform = ''; }, 150);
            });

            btnFinish.addEventListener('click', function() {
                alert('🎉 TERIMA KASIH SAYANG! HAPPY BIRTHDAY! ❤️🎂');
                this.style.transform = 'scale(0.9)';
                setTimeout(() => { this.style.transform = ''; }, 150);
            });

            // ===== INIT =====
            loadQuiz(0);
            showPage('page1');

            // Fix untuk tampilan HP agar tidak terpotong
            window.addEventListener('resize', function() {
                // Scroll ke atas jika diperlukan
                if (document.querySelector('.page.active')) {
                    // biarkan saja
                }
            });

        })();
    </script>

</body>
</html>
