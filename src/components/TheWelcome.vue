<script setup>
import { ref } from "vue";

const like = ref(0);

function likeClick() {
  like.value++;
}
function likeClick2(){
  like.value--;
}
</script>

<template>
  <div>
    <button class="button" @click="likeClick()">
      <img
        src="http://localhost:5173/"
        width="40"
        height="40"
        aly="like"
      />
    </button>
    <big style="margin:10px">{{ like }}</big>
    <button class="button2" @click="likeClick2()">
      <img
        src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fpixabay.com%2Fth%2Fillustrations%2F%25E0%25B8%259E%25E0%25B8%25B7%25E0%25B9%2589%25E0%25B8%2599%25E0%25B8%25AB%25E0%25B8%25A5%25E0%25B8%25B1%25E0%25B8%2587-%25E0%25B8%2598%25E0%25B8%25A3%25E0%25B8%25A3%25E0%25B8%25A1%25E0%25B8%258A%25E0%25B8%25B2%25E0%25B8%2595%25E0%25B8%25B4-%25E0%25B8%25A0%25E0%25B8%25B9%25E0%25B8%25A1%25E0%25B8%25B4%25E0%25B8%259B%25E0%25B8%25A3%25E0%25B8%25B0%25E0%25B9%2580%25E0%25B8%2597%25E0%25B8%25A8-7485228%2F&psig=AOvVaw3Ckm25fi8rzIcSnSEh7r9i&ust=1674481736398000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCNCSgdyo2_wCFQAAAAAdAAAAABAJ"
        width="40"
        height="40"
        aly="sad"
      />
    </button>
  </div>
</template>

<style scoped>
.button {
  background-color: lime;
  transition-duration: 0.3s;
}
.button:hover {
  box-shadow: 0 0 3px 2px darkgray;
  background-color: rgb(0, 224, 0);
}
.button:active {
  box-shadow: 0 0 4px 2px gray;
}
.button2 {
  background-color: rgb(255, 128, 128);
  transition-duration: 0.3s;
}
.button2:hover {
  box-shadow: 0 0 3px 2px darkgray;
  background-color: rgb(255, 64, 64);
}
.button2:active {
  box-shadow: 0 0 4px 2px gray;
}
</style>