<script>
export default {
  methods: {
    mudarDados() {
      const playload = {
        nome: "outro nome",
        email: "outro@email.com",
        level: "usuario-raso"
      };

      this.$store.commit("CHANGE_USER", playload);
    }
  }
};
</script>


<template>
    <div>
        <button @click="mudarDados">Mudar dados do Usario</button>
    </div>
</template>
