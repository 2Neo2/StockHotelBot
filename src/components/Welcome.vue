<template>
  <div class="welcome-screen">
    <div class="logo">
      <img src="/logo.png" alt="StockHotelBot" />
      <span class="logo-text">Stock<br />Hotel<br />Bot</span>
    </div>

    <h1>ДОБРО ПОЖАЛОВАТЬ<br />В <span class="brand">STOCKHOTELBOT</span>!</h1>
    <p class="subtitle">Бронируйте отели <span class="highlight">быстро и выгодно</span>!</p>

    <div class="tagline-buttons">
      <span>удобно</span>
      <span>мгновенно</span>
      <span>в Telegram</span>
    </div>

    <div class="graphics">
      <img class="bell" src="/bell.png" alt="bell" />
      <img class="bed" src="/bed.png" alt="bed" />
    </div>

    <button class="start-btn" @click="goNext">
      ПОЕХАЛИ! <span class="icon">▶</span>
    </button>
  </div>
</template>

<script setup>
const goNext = () => {
  // логика перехода к следующему экрану
  // например: router.push('/booking')
}
</script>

<style scoped>
.welcome-screen {
  background: #0079ff;
  color: white;
  text-align: center;
  padding: 20px;
  font-family: 'Arial', sans-serif;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.logo {
  display: flex;
  align-items: center;
  gap: 10px;
  justify-content: center;
}

.logo img {
  width: 48px;
  height: 48px;
}

.logo-text {
  font-weight: bold;
  font-size: 16px;
  line-height: 1;
}

h1 {
  font-size: 24px;
  font-weight: 800;
}

.brand {
  color: #fff;
}

.subtitle {
  font-size: 16px;
  margin-top: 10px;
}

.highlight {
  color: #ffa500;
  font-weight: bold;
}

.tagline-buttons {
  display: flex;
  justify-content: center;
  gap: 12px;
  margin: 20px 0;
}

.tagline-buttons span {
  background: white;
  color: #333;
  padding: 8px 14px;
  border-radius: 16px;
  font-weight: 600;
  font-size: 14px;
}

.graphics {
  display: flex;
  justify-content: center;
  align-items: flex-end;
  gap: 20px;
}

.graphics img {
  width: 80px;
}

.start-btn {
  background: #ffa500;
  border: none;
  border-radius: 25px;
  padding: 16px 30px;
  font-size: 18px;
  font-weight: bold;
  color: white;
  margin-top: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.2);
}

.icon {
  background: white;
  color: #ffa500;
  border-radius: 50%;
  padding: 4px 8px;
  font-weight: bold;
}
</style>
