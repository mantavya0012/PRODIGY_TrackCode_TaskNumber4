# PRODIGY_TrackCode_TaskNumber4
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Info Post Carousel</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: linear-gradient(135deg, #fbc2eb, #a6c1ee);
    }

    .carousel-container {
      width: 320px;
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(10px);
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.2);
    }

    .carousel {
      display: flex;
      transition: transform 0.5s ease-in-out;
    }

    .slide {
      min-width: 320px;
      padding: 20px;
      text-align: center;
      color: #fff;
    }

    .slide h2 {
      font-size: 1.5rem;
      margin-bottom: 10px;
    }

    .slide p {
      font-size: 1rem;
      margin: 5px 0;
    }

    .controls {
      display: flex;
      justify-content: center;
      gap: 10px;
      padding: 10px;
      background: rgba(255, 255, 255, 0.1);
    }

    .controls button {
      background: #fff;
      border: none;
      border-radius: 50%;
      width: 30px;
      height: 30px;
      cursor: pointer;
      font-weight: bold;
      transition: transform 0.2s ease;
    }

    .controls button:hover {
      transform: scale(1.1);
    }
  </style>
</head>
<body>
  <div class="carousel-container">
    <div class="carousel" id="carousel">
      <div class="slide">
        <h2>Influencer: CarryMinati</h2>
        <p><strong>Followers:</strong> 42M</p>
        <p><strong>Niche:</strong> Roasting & Comedy</p>
        <p><strong>Key Stats:</strong> YouTube #1 in India</p>
      </div>
      <div class="slide">
        <h2>Influencer: TechBurner</h2>
        <p><strong>Followers:</strong> 10M</p>
        <p><strong>Niche:</strong> Tech Reviews</p>
        <p><strong>Key Stats:</strong> Creative Content</p>
      </div>
      <div class="slide">
        <h2>Influencer: Bhuvan Bam</h2>
        <p><strong>Followers:</strong> 25M</p>
        <p><strong>Niche:</strong> Comedy & Music</p>
        <p><strong>Key Stats:</strong> BB Ki Vines Creator</p>
      </div>
    </div>
    <div class="controls">
      <button onclick="prevSlide()">&#8592;</button>
      <button onclick="nextSlide()">&#8594;</button>
    </div>
  </div>

  <script>
    let index = 0;

    function showSlide() {
      const carousel = document.getElementById('carousel');
      carousel.style.transform = `translateX(-${index * 320}px)`;
    }

    function nextSlide() {
      const totalSlides = document.querySelectorAll('.slide').length;
      index = (index + 1) % totalSlides;
      showSlide();
    }

    function prevSlide() {
      const totalSlides = document.querySelectorAll('.slide').length;
      index = (index - 1 + totalSlides) % totalSlides;
      showSlide();
    }
  </script>
</body>
</html>
