<template>
  <div class="wrapper">
    <div class="zoom-effect-container">
      <div class="image-card">
        <img :src="image" alt="Bild">
      </div>
    </div>
    <div class="white-box-text">
      <div class="text">
        <span class="title">{{ title }}</span>
        <br>
        <span class="summary">{{ summary }}</span>
      </div>
    </div>
    <div class="overlay">
      <div class="excerptHeader">
        <span>{{ excerptHeader }}</span>
        <br>
      </div>
      <div class="excerpt">
        <span>{{ excerpt }}</span>
      </div>
      <div class="btn-container">
        <a type="button" class="btn btn-primary" :href="articlePath">Artikel lesen</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Article",
  props: {
    title: String,
    summary: String,
    excerptHeader: String,
    excerpt: String,
    imgPath: String,
    articlePath: String
  },
  data() {
    return {
      image: null
    };
  },
  mounted() {
    if (this.imgPath) {
      const images = require("@/assets/" + this.imgPath);
      this.image = images;
    }
  }
};
</script>

<style>
.wrapper {
  position: relative;
  width: 450px;
  height: 580px;
  overflow: hidden;
  margin-top: 10px;
  margin-bottom: -10rem;
}
.wrapper:nth-of-type(2) {
  margin-top: calc(98px + 10px);
}
.wrapper:nth-of-type(3) {
  margin-top: 110px;
}
.wrapper:nth-of-type(4) {
  margin-top: 200px;
}

@media screen and (max-width: 940px) {
  .wrapper {
    margin-top: 50px;
  }
  .wrapper:nth-of-type(2) {
    margin-top: 140px;
  }
  .wrapper:nth-of-type(3) {
    margin-top: 140px;
  }
  .wrapper:nth-of-type(4) {
    margin-top: 140px;
  }
}

/*.wrapper .text {
    position: absolute;
    bottom: 80px;
    left: 7%;
    opacity: 1;
}*/

.wrapper:hover .text {
  opacity: 0;
}
.wrapper .text span:first-child {
  color: #004853;
  font-size: 1.36rem;
}
.wrapper .text span {
  color: #004853;
  font-size: 0.95rem;
}
.zoom-effect-container {
  width: 100%;
  height: 100%;
}

.image-card img {
  -webkit-transition: 0.4s ease;
  transition: 0.4s ease;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  opacity: 0;
  transition: 0.1s ease;
  background-color: #f63700;
  z-index: 100;
}

.white-box-text {
  background-color: white;
  z-index: 100;
  height: 135px;
  width: 350px;
  position: absolute;
  bottom: 0%;
}
.white-box-text .text {
  position: relative;
  left: 0%;
  top: 2%;
}

.btn {
  position: absolute;
  bottom: 15%;
  opacity: 1;
}
.btn-primary {
  color: #f63700;
}
.btn-primary:hover {
  color: black;
}
.excerptHeader {
  color: white;
  font-size: 2rem;
  position: relative;
  top: 2%;
  text-align: center;
}
.excerpt {
  color: white;
  position: relative;
  font-size: 1.2rem;
  text-align: center;
  margin-top: 30px;
  margin-right: 20px;
  margin-left: 20px;
  margin-bottom: 35px;
}

.btn-container .btn {
  position: relative;
  left: 35%;
}

.wrapper:hover .white-box-text {
  opacity: 0;
}

.wrapper:hover .overlay {
  opacity: 0.85;
}
.wrapper:hover .overlay .btn {
  opacity: 1;
}
.wrapper:hover .text {
  opacity: 0;
}
.wrapper:hover .image-card img {
  -webkit-transform: scale(1.12);
  transform: scale(1.12);
}

@media screen and (max-width: 960px) {
  .wrapper {
    margin-top: -2rem;
  }
}
</style>


