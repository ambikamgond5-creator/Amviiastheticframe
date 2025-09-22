# Amviiastheticframe
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>amvii</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600&display=swap" rel="stylesheet">
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: 'Poppins', sans-serif;
      overflow: hidden;
    }

    /* Moving background */
    body {
      background: url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?ixlib=rb-4.0.3&auto=format&fit=crop&w=2000&q=80') 
                  repeat center center/cover;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      flex-direction: column;
      padding: 20px;
      animation: skyMove 40s linear infinite;
    }

    /* Main title */
    h1 {
      font-size: 5em;
      color: #7b2cbf;
      text-shadow: 0 0 15px rgba(123,44,191,0.9), 0 0 30px rgba(255,255,255,0.6);
      margin: 0;
      opacity: 0;
      animation: zoomIn 2s ease forwards, float 6s ease-in-out infinite;
    }

    /* Tagline */
    p {
      font-size: 1.3em;
      color: white;
      margin-top: 15px;
      margin-bottom: 20px;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.4);
      opacity: 0;
      animation: fadeInUp 2s ease forwards;
      animation-delay: 1s;
    }

    /* Promotion line */
    .promo {
      font-size: 1.2em;
      color: #ffe4e1;
      margin-bottom: 25px;
      font-weight: 500;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.5);
      opacity: 0;
      animation: fadeInUp 2s ease forwards;
      animation-delay: 2s;
    }

    /* Button container */
    .buttons, .social {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
      margin-bottom: 30px;
      opacity: 0;
      animation: fadeInUp 2s ease forwards;
    }

    .buttons { animation-delay: 3s; }
    .social { animation-delay: 4s; }

    /* Circle buttons */
    .buttons a, .social a {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 1.5em;
      text-decoration: none;
      color: white;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
      transition: all 0.3s ease, box-shadow 0.3s ease;
      animation: float 6s ease-in-out infinite;
    }

    /* Glow on hover */
    .buttons a:hover, .social a:hover {
      transform: translateY(-4px) scale(1.1);
      box-shadow: 0 0 20px rgba(255,255,255,0.9);
    }

    /* Contact button colors */
    .email { background: #7b2cbf; }
    .whatsapp { background: #25D366; }

    /* Social button colors */
    .instagram { background: #E1306C; }
    .youtube { background: #FF0000; }
    .pinterest { background: #BD081C; }
    .shop { background: #ff9800; }

    /* Animations */
    @keyframes fadeInUp {
      from { opacity: 0; transform: translateY(30px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes zoomIn {
      from { opacity: 0; transform: scale(0.5); }
      to { opacity: 1; transform: scale(1); }
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    @keyframes skyMove {
      from { background-position: 0 0; }
      to { background-position: 1000px 0; }
    }
  </style>
</head>
<body>
  <div>
    <h1>amvii</h1>
    <p>✨ Aesthetic vibes coming soon ✨</p>
    <div class="promo">📢 Contact for any paid promotions</div>

    <!-- Contact Buttons -->
    <div class="buttons">
      <a href="mailto:ambikamgond5@gmail.com" class="email"><i class="fas fa-envelope"></i></a>
      <a href="https://wa.me/919481368624" target="_blank" class="whatsapp"><i class="fab fa-whatsapp"></i></a>
    </div>

    <!-- Social Media Links -->
    <div class="social">
      <a href="https://instagram.com/" target="_blank" class="instagram"><i class="fab fa-instagram"></i></a>
      <a href="https://youtube.com/" target="_blank" class="youtube"><i class="fab fa-youtube"></i></a>
      <a href="https://pinterest.com/" target="_blank" class="pinterest"><i class="fab fa-pinterest"></i></a>
      <a href="https://shopify.com/" target="_blank" class="shop"><i class="fas fa-shopping-bag"></i></a>
    </div>
  </div>
</body>
</html>
