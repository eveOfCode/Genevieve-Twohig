<template>
  <div class="home">
    <About />
    <Name />
    <Skills />
    <Work />
    <Fun />
    <Contact />
  </div>
</template>

<script>
// @ is an alias to /src
import About from "@/components/About";
import Name from "@/components/Name";
import Skills from "@/components/Skills";
import Contact from "@/components/Contact";
import Work from "@/components/Work";
import Fun from "@/components/Fun";

export default {
  name: "home",
  components: {
    About,
    Name,
    Skills,
    Contact,
    Work,
    Fun
  }
};
</script>
