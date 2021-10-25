<template>
  <div>
    <Navbar id="navbar" />
    <Nuxt />
    <div class="scrollup" fixed></div>
    <Footer id="footer" />
  </div>
</template>

<style>
.scrollup {
  position: fixed;
  left: 98%;
  bottom: 100px;
  z-index: 100;
}
.scrollup a {
  /*描画位置*/
  position: absolute;
  right: 10px;
  top: 40px;
  /*テキストの形状*/
  color: #000;
  font-size: 0.7rem;
  letter-spacing: 0.05em;
}
.scrollup::after {
  content: '';
  /*描画位置*/
  position: absolute;
  top: 0;
  /*線の形状*/
  width: 1px;
  height: 100px;
  background: #000;
  animation: pathup 3s ease-in-out infinite;
  opacity: 0;
}
</style>