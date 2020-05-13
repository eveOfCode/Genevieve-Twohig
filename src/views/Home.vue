<template>
  <div class="home">
    <FirstPage />
    <About />
    <Skills />
    <Work />
    <Fun />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import FirstPage from "@/components/FirstPage";
import About from "@/components/About";
import Skills from "@/components/Skills";
import Contact from "@/components/Contact";
import Work from "@/components/Work";
import Fun from "@/components/Fun";

export default {
  name: "home",
  components: {
    FirstPage,
    About,
    Skills,
    Contact,
    Work,
    Fun
  }
};
</script>
