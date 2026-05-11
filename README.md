/* =========================================
   AETHELGARD ARŞİVLERİ - KADİM STİL DOSYASI
   ========================================= */

/* Fontların Çağırılması */
@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;700&family=Crimson+Text:ital,wght@0,400;0,700;1,400&display=swap');

body {
    margin: 0;
    padding: 0;
    background-color: #050a1a;
    /* Arka plan görseli emrettiğiniz gibi image_0.png */
    background-image: 
        linear-gradient(rgba(5, 10, 26, 0.85), rgba(5, 10, 26, 0.95)),
        url('image_0.png');
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
    color: #e0e0e0;
    font-family: 'Cinzel', serif;
    overflow-x: hidden;
    /* Özel İmleç Büyüsü */
    cursor: url('https://img.icons8.com/ios-filled/20/74b9ff/sparkling-diamond.png'), auto;
}

/* Arka Plandaki Büyü Tozları */
#particles-js {
    position: fixed;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    z-index: 1;
    pointer-events: none;
}

/* Ana Konteyner */
.container {
    max-width: 850px;
    margin: 40px auto;
    padding: 30px;
    background: rgba(10, 20, 45, 0.6);
    border: 1px solid rgba(116, 185, 255, 0.2);
    box-shadow: 0 0 50px rgba(0, 0, 0, 0.8);
    position: relative;
    z-index: 2;
    border-radius: 8px;
}

/* Başlık Stili */
h1 {
    text-align: center;
    color: #74b9ff;
    text-shadow: 0 0 15px rgba(116, 185, 255, 0.6);
    font-size: 2.8em;
    margin-bottom: 10px;
    letter-spacing: 3px;
}

/* Kitap Başlıkları (Butonlar) */
.kitap-baslik {
    background: rgba(10, 20, 45, 0.8);
    border: 1px solid #1a3a6d;
    padding: 20px;
    margin: 15px 0;
    cursor: pointer;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    text-align: center;
    font-weight: bold;
    letter-spacing: 2px;
    text-transform: uppercase;
    position: relative;
}

.kitap-baslik:hover {
    border-color: #74b9ff;
    box-shadow: 0 0 25px rgba(116, 185, 255, 0.4);
    transform: scale(1.03);
    background: rgba(20, 40, 80, 0.9);
}

/* ANTİK PARŞÖMEN ALANI */
.bolumler {
    display: none;
    background-color: #e4d5b7; /* Antik kağıt tonu */
    background-image: url('https://www.transparenttextures.com/patterns/paper-fibers.png'); /* Kağıt dokusu */
    padding: 30px;
    border-radius: 2px;
    box-shadow: 
        inset 0 0 50px #c3a67d, 
        0 10px 30px rgba(0,0,0,0.7);
    font-family: 'Crimson Text', serif;
    border: 1px solid #d4b483;
    margin-top: -15px;
    position: relative;
    z-index: 3;
}

/* Parşömen Giriş Yazısı */
.bolumler p {
    color: #5d4037;
    border-bottom: 2px solid rgba(93, 64, 55, 0.3);
    padding-bottom: 10px;
    margin-bottom: 20px;
    font-style: italic;
    font-weight: bold;
    text-align: center;
}

/* BÖLÜM LİNKLERİ (Mürekkep Etkisi) */
.bolum-link {
    display: block;
    padding: 12px;
    color: #3b2b1d !important; /* Net okunan mürekkep rengi */
    text-decoration: none;
    border-bottom: 1px dashed rgba(59, 43, 29, 0.3);
    font-weight: 700;
    font-size: 1.25em;
    transition: all 0.3s ease;
}

.bolum-link:hover {
    color: #8b0000 !important; /* Kan kırmızısı vurgu */
    background: rgba(0, 0, 0, 0.05);
    padding-left: 25px;
}

/* MOBİL UYUM BÜYÜSÜ */
@media (max-width: 768px) {
    .container {
        width: 92%;
        margin: 15px auto;
        padding: 20px 15px;
    }

    h1 {
        font-size: 1.8em;
        letter-spacing: 1px;
    }

    .kitap-baslik {
        padding: 15px;
        font-size: 0.9em;
    }

    .bolumler {
        padding: 20px 15px;
        font-size: 1.15em;
    }

    body {
        cursor: default; /* Mobilde dokunmatik kullanım için imleci sıfırlar */
    }
}
