---
title: "Portfolio item number 1"
excerpt: "Short description of portfolio item number 1<br/><img src='images/mapa1.png'>"
collection: portfolio
---

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Carousel Example</title>
<style>
    .carousel-container {
        width: 100%;
        overflow: hidden;
        position: relative;
    }

    .carousel-slide {
        display: flex;
        transition: transform 0.5s ease;
    }

    .carousel-item {
        width: 100%;
        flex: 0 0 auto;
    }
</style>
</head>
<body>

<div class="carousel-container">
    <div class="carousel-slide">
        <img class="carousel-item" src='images/mapa1.png' alt="Mapa 1">
        <img class="carousel-item" src='images/mapa2.png' alt="Mapa 2">
        <img class="carousel-item" src='images/mapa3.png' alt="Mapa 3">
        <img class="carousel-item" src='images/mapa4.png' alt="Mapa 4">
        <img class="carousel-item" src='images/mapa5.png' alt="Mapa 5">
        <img class="carousel-item" src='images/mapa6.png' alt="Mapa 6">
        <img class="carousel-item" src='images/mapa7.png' alt="Mapa 7">
    </div>
</div>

<script>
    const carouselSlide = document.querySelector('.carousel-slide');
    const carouselItems = document.querySelectorAll('.carousel-item');

    let counter = 0;

    function nextSlide() {
        if (counter === carouselItems.length - 1) return;
        counter++;
        carouselSlide.style.transform = `translateX(${-counter * 100}%)`;
    }

    function prevSlide() {
        if (counter === 0) return;
        counter--;
        carouselSlide.style.transform = `translateX(${-counter * 100}%)`;
    }

    setInterval(nextSlide, 3000); // Auto slide every 3 seconds
</script>

</body>
</html>