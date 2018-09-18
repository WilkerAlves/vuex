<script>
import WwButton from "../button";

export default {
  components: {
    WwButton
  },
  computed: {
    email() {
      return this.$store.state.user.email;
    }
  }
};
</script>



<template>
    <div>
        Email: {{email}}
        <ww-button></ww-button>
    </div>
</template>
