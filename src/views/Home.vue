<template>
  <div class="home">
    <Name />
    <About />
    <Skills />
    <Work />
    <Fun />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import Name from "@/components/Name";
import About from "@/components/About";
import Skills from "@/components/Skills";
import Contact from "@/components/Contact";
import Work from "@/components/Work";
import Fun from "@/components/Fun";

export default {
  name: "home",
  components: {
    Name,
    About,
    Skills,
    Contact,
    Work,
    Fun
  }
};
</script>
