<template>
  <v-card>
    <v-img src="/TopBanner.jpg">
      <v-layout justify-center align-center text-center fill-height white--text>
        <h1 class="slogan">Curious. Creative. Consistent.</h1>
        <div style="margin-top: 100px" class="icon-scroll"></div>
      </v-layout>
      <!-- <v-layout
        fill-height=""
        class="pb-5"
        text-center
        justify-center=""
        align-end=""
      >
        <div class=" icon-scroll"></div>
      </v-layout> -->
    </v-img>
  </v-card>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style>
.icon-scroll,
.icon-scroll:before {
  position: absolute;
  /* left: 50%; */
}
.icon-scroll {
  width: 60px;
  height: 120px;
  /* margin-left: -20px */
  /* top: 50% */
  /* margin-top: -35px */
  /* border: 0px solid transparent; */
  /* box-shadow: inset 0 0 0 1px #fff; */
  border-radius: 25px;
}

.icon-scroll:before {
  content: "↓";
  width: 36px;
  color: grey;
  font-size: 2em;
  height: 48px;
  background: #fff;
  margin-left: -10px;
  top: 8px;
  border-radius: 10px;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  animation-name: scroll;
}

@keyframes scroll {
  0% {
    opacity: 1;
  }
  100% {
    opacity: 0;
    transform: translateY(80px);
  }
}
</style>
