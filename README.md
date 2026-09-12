<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>READINGLAND - Your Cozy Reading Corner</title>
  
  <!-- Google Fonts: Fredoka cho chữ bóng bọt 3D, Nunito cho nội dung -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@600;700;800&family=Nunito:wght@600;700;800&display=swap" rel="stylesheet">
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <style>
    /* Font tùy chỉnh */
    body {
      font-family: 'Nunito', sans-serif;
      background: linear-gradient(135deg, #FFF5F5 0%, #EBF8FF 50%, #F0FFF4 100%);
    }
    
    .font-bubble {
      font-family: 'Fredoka', cursive;
    }

    /* Hiệu ứng Chữ Nổi 3D Pastel (Bubble Text) */
    .bubble-title {
      color: #FF7B9C;
      text-shadow: 
        3px 3px 0px #FFC2D1,
        6px 6px 0px #FFE5EC,
        9px 9px 15px rgba(255, 123, 156, 0.3);
      letter-spacing: 2px;
    }

    /* Hiệu ứng Nút Bấm 3D Nẩy (Press Effect) */
    .btn-3d {
      transition: all 0.15s ease;
      box-shadow: 0px 8px 0px var(--shadow-color);
    }
    
    .btn-3d:hover {
      transform: translateY(-2px);
      box-shadow: 0px 10px 0px var(--shadow-color);
    }
    
    .btn-3d:active {
      transform: translateY(6px);
      box-shadow: 0px 2px 0px var(--shadow-color);
    }

    /* Đĩnh nghĩa màu bóng 3D cho từng nút */
    .btn-primary {
      background-color: #FF9B9B;
      color: #FFFFFF;
      --shadow-color: #FF6868;
    }

    .btn-secondary-1 {
      background-color: #A8E6CF;
      color: #2D5A46;
      --shadow-color: #72C3A5;
    }

    .btn-secondary-2 {
      background-color: #FFD3B6;
      color: #6C4427;
      --shadow-color: #FFAAA6;
    }

    .btn-secondary-3 {
      background-color: #D4A5A5;
      color: #FFFFFF;
      --shadow-color: #9E7676;
    }

    /* Hiệu ứng mây trôi nhẹ bồng bềnh */
    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-10px) rotate(2deg); }
    }
    
    .floating {
      animation: float 4s ease-in-out infinite;
    }
  </style>
</head>

<body class="min-h-screen flex flex-col items-center justify-center p-6 relative overflow-hidden text-gray-700">

  <!-- Họa tiết mây trôi trang trí góc màn hình -->
  <div class="absolute top-10 left-10 text-5xl opacity-40 floating">☁️</div>
  <div class="absolute top-20 right-12 text-4xl opacity-40 floating" style="animation-delay: 1.5s;">✨</div>
  <div class="absolute bottom-12 left-16 text-4xl opacity-40 floating" style="animation-delay: 2s;">📖</div>
  <div class="absolute bottom-16 right-16 text-5xl opacity-40 floating" style="animation-delay: 0.8s;">☁️</div>

  <!-- Bố cục Trung tâm -->
  <main class="max-w-2xl w-full text-center z-10 flex flex-col items-center">
    
    <!-- Tiêu đề Welcome siêu nhỏ xinh -->
    <span class="inline-block px-4 py-1.5 mb-3 text-sm font-bold text-pink-500 bg-pink-100 rounded-full tracking-wider uppercase shadow-sm">
      ✨ Welcome to ✨
    </span>

    <!-- Tiêu đề chính READINGLAND Chữ Nổi 3D -->
    <h1 class="font-bubble text-6xl md:text-8xl font-black bubble-title mb-3 select-none">
      READINGLAND
    </h1>

    <!-- Dòng mô tả theo đúng yêu cầu -->
    <p class="text-xl md:text-2xl font-bold text-gray-500 mb-10 tracking-wide">
      Your cozy reading corner 📖✨
    </p>

    <!-- Nút Bắt đầu chính (Primary Action) -->
    <div class="w-full max-w-sm mb-8">
      <a href="addnewarticle.html" class="btn-3d btn-primary w-full py-4 px-8 rounded-3xl text-xl font-extrabold flex items-center justify-center gap-3 no-underline inline-block">
        <span class="text-2xl">➕</span>
        <span>Add New Article</span>
      </a>
    </div>

    <!-- Các Nút Phụ Bên Dưới (Secondary Actions) -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 w-full">
      
      <!-- Nút Thư viện -->
      <a href="mylibrary.html" class="btn-3d btn-secondary-1 py-3 px-4 rounded-2xl font-extrabold flex items-center justify-center gap-2 no-underline">
        <span class="text-xl">📚</span>
        <span>My Library</span>
      </a>

      <!-- Nút Sổ từ vựng -->
      <a href="vocabularynotebook.html" class="btn-3d btn-secondary-2 py-3 px-4 rounded-2xl font-extrabold flex items-center justify-center gap-2 no-underline">
        <span class="text-xl">📇</span>
        <span>Vocabulary Notebook</span>
      </a>

      <!-- Nút Tiến độ -->
      <a href="myprogress.html" class="btn-3d btn-secondary-3 py-3 px-4 rounded-2xl font-extrabold flex items-center justify-center gap-2 no-underline">
        <span class="text-xl">📊</span>
        <span>My Progress</span>
      </a>

    </div>

  </main>

</body>
</html>
