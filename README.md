<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pengumuman Kelulusan MTs Falakhiyah</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f5f7fa;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 2rem 0;
            text-align: center;
            border-radius: 0 0 20px 20px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            margin-bottom: 2rem;
        }
        
        .logo {
            width: 100px;
            height: 100px;
            margin-bottom: 1rem;
            border-radius: 50%;
            border: 3px solid white;
            object-fit: cover;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
        }
        
        .year {
            display: inline-block;
            background-color: var(--accent);
            padding: 0.3rem 1rem;
            border-radius: 20px;
            font-weight: 700;
            margin-top: 1rem;
            font-size: 1.1rem;
        }
        
        .search-box {
            background-color: white;
            max-width: 600px;
            margin: 2rem auto;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
        }
        
        .search-box h2 {
            color: var(--primary);
            margin-bottom: 1.5rem;
        }
        
        .input-group {
            display: flex;
            margin-bottom: 1rem;
        }
        
        input[type="text"] {
            flex: 1;
            padding: 12px 15px;
            border: 2px solid #ddd;
            border-radius: 5px 0 0 5px;
            font-size: 1rem;
            transition: all 0.3s;
        }
        
        input[type="text"]:focus {
            border-color: var(--secondary);
            outline: none;
        }
        
        button {
            background-color: var(--secondary);
            color: white;
            border: none;
            padding: 0 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s;
        }
        
        button:hover {
            background-color: #2980b9;
        }
        
        .result {
            display: none;
            background-color: white;
            max-width: 600px;
            margin: 2rem auto;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
            animation: fadeIn 0.5s ease;
        }
        
        .result h3 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .result p {
            margin-bottom: 0.5rem;
        }
        
        .lulus {
            color: #27ae60;
            font-weight: 700;
            font-size: 1.5rem;
            margin: 1rem 0;
        }
        
        .tidak-lulus {
            color: var(--accent);
            font-weight: 700;
            font-size: 1.5rem;
            margin: 1rem 0;
        }
        
        .student-info {
            text-align: left;
            background-color: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            margin-top: 1.5rem;
        }
        
        .student-info p {
            margin-bottom: 0.8rem;
            display: flex;
        }
        
        .student-info p span:first-child {
            font-weight: 600;
            width: 150px;
            display: inline-block;
        }
        
        .congrats {
            font-size: 1.2rem;
            margin-top: 1.5rem;
            color: var(--primary);
        }
        
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 3rem 0;
        }
        
        .stat-box {
            background-color: white;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
            flex: 1;
            margin: 0.5rem;
            min-width: 200px;
        }
        
        .stat-box h3 {
            color: var(--secondary);
            margin-bottom: 0.5rem;
        }
        
        .stat-box p {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            background-color: var(--primary);
            color: white;
            margin-top: 3rem;
        }
        
        .social-icons {
            margin: 1rem 0;
        }
        
        .social-icons a {
            color: white;
            margin: 0 10px;
            font-size: 1.5rem;
            transition: all 0.3s;
        }
        
        .social-icons a:hover {
            color: var(--secondary);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            .subtitle {
                font-size: 1rem;
            }
            
            .search-box, .result {
                padding: 1.5rem;
            }
            
            .input-group {
                flex-direction: column;
            }
            
            input[type="text"] {
                border-radius: 5px;
                margin-bottom: 10px;
            }
            
            button {
                border-radius: 5px;
                padding: 12px;
            }
            
            .stats {
                flex-direction: column;
            }
            
            .stat-box {
                margin-bottom: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <img src="https://via.placeholder.com/100" alt="Logo MTs Falakhiyah" class="logo">
            <h1>MTs FALAKHIYAH</h1>
            <p class="subtitle">Pengumuman Kelulusan Peserta Didik</p>
            <div class="year">2024</div>
        </div>
    </header>
    
    <div class="container">
        <div class="search-box">
            <h2>Cek Status Kelulusan</h2>
            <div class="input-group">
                <input type="text" id="nisn" placeholder="Masukkan NISN Anda" required>
                <button id="search-btn"><i class="fas fa-search"></i> Cari</button>
            </div>
            <p>Masukkan Nomor Induk Siswa Nasional (NISN) Anda untuk melihat status kelulusan</p>
        </div>
        
        <div class="result" id="result">
            <!-- Hasil akan muncul di sini -->
        </div>
        
        <div class="stats">
            <div class="stat-box">
                <h3>Total Siswa</h3>
                <p id="total-siswa">120</p>
            </div>
            <div class="stat-box">
                <h3>Lulus</h3>
                <p id="lulus">115</p>
            </div>
            <div class="stat-box">
                <h3>Tidak Lulus</h3>
                <p id="tidak-lulus">5</p>
            </div>
            <div class="stat-box">
                <h3>Persentase</h3>
                <p id="persentase">95.83%</p>
            </div>
        </div>
    </div>
    
    <footer>
        <div class="container">
            <h3>MTs Falakhiyah</h3>
            <p>Jl. Pendidikan No. 123, Kec. Falakhiyah, Kab. Falakhiyah</p>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
            <p>&copy; 2024 MTs Falakhiyah. Semua Hak Dilindungi.</p>
        </div>
    </footer>
    
    <script>
        // Data dummy siswa (dalam aplikasi nyata, ini akan diambil dari database)
        const students = [
            { nisn: "1234567890", name: "Ahmad Fauzi", kelas: "IX-A", nilai: 85, status: "LULUS" },
            { nisn: "2345678901", name: "Siti Aminah", kelas: "IX-B", nilai: 92, status: "LULUS" },
            { nisn: "345678901
