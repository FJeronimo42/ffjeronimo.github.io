---
title: "Portfolio Teste Carrossel"
excerpt: "Short description of portfolio item number 4 <br/><img src='images/map9.png'>"
collection: portfolio
---

<style>
/* Estilos para o carrossel */
.carousel {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  scroll-behavior: smooth;
  margin-bottom: 20px;
}

.carousel__item {
  flex: 0 0 auto;
  height: 10cm; /* altura fixa */
  scroll-snap-align: start;
}

.map {
  height: 100%;
  width: auto;
  max-width: 100%; /* Garante que a largura não ultrapasse a largura do contêiner */
}
</style>

<div class="carousel">
  <div class="carousel__item">
    <img src="mapa1.png" class="map" alt="Mapa 1">
  </div>
  <div class="carousel__item">
    <img src="mapa2.png" class="map" alt="Mapa 2">
  </div>
  <div class="carousel__item">
    <img src="mapa3.png" class="map" alt="Mapa 3">
  </div>
  <div class="carousel__item">
    <img src="mapa4.png" class="map" alt="Mapa 4">
  </div>
  <div class="carousel__item">
    <img src="mapa5.png" class="map" alt="Mapa 5">
  </div>
  <div class="carousel__item">
    <img src="mapa6.png" class="map" alt="Mapa 6">
  </div>
  <div class="carousel__item">
    <img src="mapa7.png" class="map" alt="Mapa 7">
  </div>
</div>
