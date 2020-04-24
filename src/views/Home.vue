<template>
  <div class="home">
    <Name />
    <Skills />
    <Work />
    <Volunteer />
    <Fun />
  </div>
</template>

<script>
// @ is an alias to /src
import Name from "@/components/Name";
import Skills from "@/components/Skills";
import Volunteer from "@/components/Volunteer";
import Work from "@/components/Work";
import Fun from "@/components/Fun";

export default {
  name: "home",
  components: {
    Name,
    Skills,
    Volunteer,
    Work,
    Fun
  }
};
</script>
