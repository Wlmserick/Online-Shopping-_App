# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

## Colors

### Primary

- Soft blue: hsl(215, 51%, 70%)
- Cyan: hsl(178, 100%, 50%)

### Neutral

- Very dark blue (main BG): hsl(217, 54%, 11%)
- Very dark blue (card BG): hsl(216, 50%, 16%)
- Very dark blue (line): hsl(215, 32%, 27%)
- White: hsl(0, 0%, 100%)

## Typography

### Body Copy

- Font size (paragraph): 18px

### Font

- Family: [Outfit](https://fonts.google.com/specimen/Outfit)
- Weights: 300, 400, 600
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');
font-family: 'Outfit', sans-serif;
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    place-items: center;
    justify-content: center;
    align-items: center;
}



<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  
  <title>Frontend Mentor | NFT preview card component</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="card">
    <div class="image-container">
      <img src="images/image-equilibrium.jpg" alt="Equilibrium Image" height="300" width="300" class="crypto-image">
      <div class="overlay">
        <img src="images/icon-view.svg" alt="View Icon">
      </div>
    </div>
    <div class="detail">
      <h3 class="detail-title">Equilibrium #3429</h3>
      <p class="detail-description">Our Equilibrium collection promotes balance and calm.</p>
      <div class="price-detail">
        <div class="price-container">
          <img src="images/icon-ethereum.svg" alt="Ethereum Icon" height="16">
          <p class="price">0.041 ETH</p>
        </div>
        <div class="time">
          <img src="images/icon-clock.svg" alt="Clock Icon" height="16">
          <p class="days">3 days left</p>
        </div>
      </div>
    </div>
    <hr>
    <div class="author">
      <img src="images/image-avatar.png" alt="Author Image" width="30" height="30">
      <span class="author-span">Creation of <span class="author-name">Jules Wyvern</span></span>
    </div>
  </div>

  <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="#">Mark Angelo Cruz</a>.
  </div>
</body>
</html>







@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.attribution { 
  font-size: 11px; text-align: center; 
  color: white;
}

.attribution a { 
  color: hsl(228, 45%, 44%); 
}

body {
  background-color: hsl(217, 54%, 11%);
  font-family: 'Outfit', sans-serif;
  font-size: 18px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.card {
  background-color: hsl(216, 50%, 16%);
  display: flex;
  flex-direction: column;
  margin: 1rem;
  border-radius: 20px;
}

.crypto-image {
  border-radius: 10px;
  margin: 1.5rem;
}

.image-container {
  position: relative;
  cursor: pointer;
}

.overlay {
  position: absolute;
  background-color: hsl(178, 100%, 50%, 0.6);
  padding: 7.8rem;
  border-radius: 10px;
  top: 1.5rem;
  left: 1.5rem;
  opacity: 0;
}

.image-container:active .overlay {
  opacity: 1;
}

.detail {
  display: flex;
  flex-direction: column;
  width: 18rem;
  margin-left: 1.5rem;
  margin-right: 1.5rem;
  margin-bottom: 1.5rem;
}

.detail-title {
  color: hsl(0, 0%, 100%);
  margin-bottom: 1rem;
  cursor: pointer;
}

.detail-title:active {
  color: hsl(178, 100%, 50%);
}

.detail-description {
  color: hsl(215, 51%, 70%);
  margin-bottom: 2rem;
}

.price-detail {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.price-container {
  display: flex;
  align-items: center;
  gap: 0.3rem;
  color: hsl(178, 100%, 50%);
}

.time {
  display: flex;
  align-items: center;
  gap: 0.3rem;
}

.days {
  color: hsl(215, 51%, 70%);
}

.author {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  margin: 1.5rem;
}

.author img {
  border: 1px solid white;
  border-radius: 50%;
  margin-right: 1rem;
}

.author-span {
  color: hsl(215, 51%, 70%);
  font-size: 14px;
}

.author-name {
  color: white;
  cursor: pointer;
}

.author-name:active {
  color: hsl(178, 100%, 50%);
}

hr {
  border-bottom: 1px solid hsl(215, 32%, 27%);
  margin-left: 1.5rem;
  margin-right: 1.5rem;
}
