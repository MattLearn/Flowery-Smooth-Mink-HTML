<template>
  <div class="home-container">
    <div id="menu" class="home-container1">
      <h1 class="home-text">RGB Gradient Randomizer</h1>
      <div class="home-container2">
        <button id="btn-red" type="button" class="home-button color-shift button">
          Red
        </button>
        <button
          id="btn-blue"
          type="button"
          class="home-button1 color-shift button"
        >
          Blue
        </button>
        <button
          id="btn-green"
          type="button"
          class="home-button2 color-shift button"
        >
          Green
        </button>
      </div>
    </div>
    <div id="viewBg" class="home-container3"></div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  metaInfo: {
    title: 'RGB Gradient Generator',
    meta: [
      {
        property: 'og:title',
        content: 'RGB Gradient Generator',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  display: flex;
  overflow: auto;
  min-height: 100vh;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.home-container1 {
  flex: 1;
  width: 25%;
  height: 100%;
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: flex-start;
  background-color: rgba(217, 217, 217, 0.5);
}
.home-text {
  margin-top: var(--dl-space-space-sixunits);
  text-align: center;
  margin-bottom: var(--dl-space-space-sixunits);
}
.home-container2 {
  width: 200px;
  height: 290px;
  display: flex;
  align-self: center;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.home-button {
  transition: 0.3s;
}
.home-button:hover {
  background-color: #fd6666;
}
.home-button1 {
  transition: 0.3s;
}
.home-button1:hover {
  background-color: #7d83ff;
}
.home-button2 {
  transition: 0.3s;
}
.home-button2:hover {
  background-color: #a3fb8e;
}
.home-container3 {
  top: 0px;
  right: 0px;
  width: 75%;
  border: 2px dashed rgba(120, 120, 120, 0.4);
  bottom: 0px;
  height: 100%;
  margin: auto;
  display: flex;
  position: absolute;
  align-self: flex-end;
  align-items: center;
  justify-content: center;
  background-image: linear-gradient(to right, #bdc3c7 0%, #2c3e50 100%);
}
</style>
