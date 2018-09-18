<script>
import WwUser from "./components/users/main";
import { mapState } from "vuex";

export default {
  name: "app",
  components: {
    WwUser
  },
  computed: {
    ...mapState({
      user: state => {
        const { name, email } = state.user;
        return `O usuario logado é ${name} e possui o e-mail ${email}`;
      }
    })
    
  }
};
</script>



<template>
  <div>
    <h1> Bem vindo ao VUEX2</h1>
    <ww-user></ww-user>
  </div>
</template>
