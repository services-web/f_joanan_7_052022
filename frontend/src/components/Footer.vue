<template>
  <footer
    class="bottom-0 w-full bg-gray-600 shadow-lg py-6 opacity-90"
  >
    <div
      class="container mx-auto
            flex justify-center pb-3"
    >
      <router-link v-if="status == 'isConnected'" to="/wall">
        <img
          class="object-contain h-10"
          src="../assets/icons/icon-white-navbar.png"
          alt="Groupomania logo"
        />
      </router-link>
      <router-link v-else to="/">
        <img
          class="object-contain h-10"
          src="../assets/icons/icon-white-navbar.png"
          alt="Groupomania logo"
        />
      </router-link>
    </div>
    <div class="flex justify-center">
      <ul class="text-white text-center">
        <li class="flex pb-2 hover:text-green-400">
          <MailIcon class="h-6 w-5 mr-2" />
          <a href="mailto:#"> Nous contacter</a>
        </li>
        <li class="flex pb-2 hover:text-green-300">
          <AnnotationIcon class="h-6 w-5 mr-2" />
          <a href="#"> Mentions légales</a>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>
//mapState:
//Nous avons maintenant accès à l'intégralité de l' objet dans le composant, qui devient donc un composant calculé. 
import { mapState } from "vuex"; 

import { MailIcon, AnnotationIcon } from "@heroicons/vue/solid";

export default {
  components: { MailIcon, AnnotationIcon },
//Vous pouvez facilement accéder au nom d'utilisateur avec ce qui suit :
//{{status.data.name}}...
  computed: {
    ...mapState(["status"]), 
  },
};
</script>
