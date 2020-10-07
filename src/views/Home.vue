<template>
  <div class="home">
    <Presentacion/>
    <Sobremi/>
  </div>
</template>

<script>
 import Presentacion from "@/components/Presentacion.vue";
 import Sobremi from "@/components/Sobremi.vue";

export default {
  name: "Home",
  components: {
    Presentacion,
    Sobremi
  }
};
</script>
