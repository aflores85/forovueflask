
<template>
  <div>
  <hola-mundo-comp></hola-mundo-comp>
  <lista-foros></lista-foros>
  <form-foro></form-foro>
  <Lista-Subject></Lista-Subject>
  </div>
</template>

<script>
import HolaMundoComp from "../components/HolaMundoComp";
import ListaForos from "../components/ListaForos";
import FormForo from "../components/FormForo";
import ListaSubject from "../components/ListaSubject";



export default {
  name: "InicioView",
  components: { HolaMundoComp, ListaForos, FormForo, ListaSubject },
    
};
</script>

<style scoped></style>

