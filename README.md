<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Harian Mewspaper - Kucing Hilang!</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Times New Roman', serif;
            background: #f4e4bc;
            color: #333;
            line-height: 1.6;
        }
        .newspaper {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 0 30px rgba(0,0,0,0.1);
            position: relative;
        }
        /* UTih TERSEMBUNYI - Sangat halus */
        .utih-hidden {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 200px;
            font-weight: bold;
            color: rgba(255, 255, 255, 0.001); /* Hampir transparan */
            pointer-events: none;
            z-index: 1;
            user-select: none;
            mix-blend-mode: difference; /* Blend dengan background */
            line-height: 0.8;
        }
        .header {
            background: linear-gradient(90deg, #8b4513, #d2691e);
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
            z-index: 2;
        }
        .logo {
            font-size: 3em;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .date {
            font-size: 1.2em;
            opacity: 0.9;
        }
        .main-story {
            padding: 40px;
            border-bottom: 3px solid #000;
            position: relative;
            z-index: 2;
        }
        .headline {
            font-size: 3.5em;
            color: #8b0000;
            text-align: center;
            margin-bottom: 20px;
            line-height: 1.1;
            font-weight: bold;
        }
        .lead-photo {
            width: 100%;
            height: 400px;
            background: linear-gradient(45deg, #ff6b6b, #ffd93d);
            border: 5px solid #000;
            margin: 20px 0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4em;
            position: relative;
            z-index: 2;
        }
        .photo-text {
            z-index: 3;
            position: relative;
        }
        .story-body {
            font-size: 1.3em;
            margin-bottom: 30px;
        }
        .byline {
            font-style: italic;
            color: #666;
            margin-bottom: 20px;
            font-size: 1.1em;
        }
        .side-stories {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            padding: 40px;
            border-top: 3px solid #000;
        }
        .side-story {
            background: #f9f9f9;
            padding: 25px;
            border: 2px solid #ddd;
        }
        .side-headline {
            font-size: 1.8em;
            color: #8b0000;
            margin-bottom: 15px;
        }
        /* Efek tersembunyi tambahan */
        .utih-watermark {
            position: fixed;
            top: 10px;
            left: 10px;
            font-size: 12px;
            color: rgba(0,0,0,0.02);
            font-family: monospace;
            pointer-events: none;
            z-index: 999;
            animation: fadeInOut 3s infinite;
        }
        @keyframes fadeInOut {
            0%, 100% { opacity: 0.01; }
            50% { opacity: 0.03; }
        }
        @media (max-width: 768px) {
            .side-stories {
                grid-template-columns: 1fr;
            }
            .headline {
                font-size: 2.5em;
            }
            .utih-hidden {
                font-size: 120px;
            }
        }
    </style>
</head>
<body>
    <div class="newspaper">
        <!-- UTih BESAR TAPI TERSEMBUNYI DI TENGAH KORAN -->
        <div class="utih-hidden">UTIH</div>
        
        <div class="header">
            <div class="logo">📰 Harian Mewspaper</div>
            <div class="date">Senin, 25 Desember 2023 | Edisi Khusus Pencarian</div>
        </div>

        <div class="main-story">
            <div class="headline">🐱 KUCING KAMPUNG HILANG!</div>
            
            <div class="lead-photo">
                <div class="photo-text">❌ KUCING HILANG ❌</div>
            </div>

            <div class="byline">Oleh: Tim Pencari Kucing Mewspaper</div>

            <div class="story-body">
                <p><strong>Desa Kucing Harmoni</strong> - Warga desa dikejutkan dengan hilangnya kucing kampung kesayangan semua orang, <strong>"Si Utih"</strong>. Kucing berbulu putih ini terakhir terlihat pada Sabtu malam di sekitar pos ronda.</p>
                
                <p>"Kami sudah cari ke mana-mana, dari pohon kelapa sampai got sempit, tapi Utih tidak ketemu!" kata Bu RT yang terlihat menangis. "Dia kucing yang baik hati, selalu menyapa dengan 'meow' lembutnya."</p>
                
                <p>Saksi mata melaporkan melihat bayangan misterius membawa sesuatu yang berbulu putih menuju hutan belantara. Tim pencari kucing telah dikerahkan dengan membawa makanan kaleng dan mainan kucing sebagai umpan.</p>
                
                <p>Warga dimohonkan untuk melapor jika melihat kucing putih dengan ciri khas mata biru dan suka tidur di atas panci. Hadiah 1 ikan asin untuk siapa saja yang menemukan!</p>
            </div>
        </div>

        <div class="side-stories">
            <div class="side-story">
                <div class="side-headline">🐭 Tikus Makin Berani?</div>
                <p>Sejak kucing hilang, tikus-tikus mulai berani keluar siang hari. Warga khawatir stok beras akan habis!</p>
            </div>
            
            <div class="side-story">
                <div class="side-headline">🕵️‍♂️ Tim Pencari Aktif</div>
                <p>100 relawan telah bergabung dalam operasi pencarian "Utih Come Home". Mereka membawa senter, makanan kucing, dan semangat tinggi!</p>
            </div>
        </div>
    </div>

    <!-- Watermark kecil yang berkedip sangat halus di pojok -->
    <div class="utih-watermark">utih</div>

</body>
</html>
