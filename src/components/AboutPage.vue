<script setup></script>

<template>
  <div class="about" id="home">
    <div className="left-section">
      <img src="../assets/about1.jpg" alt="About" />
      <div className="text">
        <b>Booked Tool</b> enables you to<br />create Interactive Advertisement
        <button>What is it?</button>
      </div>
    </div>
    <div className="right-section">
      <img src="../assets/about2.jpg" alt="About" />
    </div>
  </div>
</template>

<style scoped>
.about {
  display: flex;
  height: 25%;
  margin-top: 70px;
}
.text {
  color: #000;
  font-size: 19px;
  width: 20%;
  left: 30%;
  position: absolute;
  top: 25%;
  text-align: left;
}
.right-section,
.left-section {
  width: 50%;
}
img {
  width: 100%;
}
@media only screen and (max-width: 900px) {
  .about {
    display: flex;
    flex-direction: column;
  }
  .text {
    color: #000;
    font-size: 19px;
    left: 65%;
    top: 50%;
  }
  .right-section,
  .left-section {
    margin: -2px;
    width: 100%;
  }
  img {
    width: 100%;
  }
}

@media only screen and (max-width: 700px) {
  .text {
    font-size: 18px;
    top: 40%;
  }
}
</style>
