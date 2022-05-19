<template>
  <div
    class="flex justify-center flex-col items-center py-10 2xl:py-24"
  >
    <div
      class="flex justify-center flex-col items-center rounded-xl shadow-lg bg-gray-50 mt-6 p-5 w-11/12 md:w-1/2"
    >
     <h1 class="text-3xl text-gray-600 md:text-6xl hover:text-green-800 ">Bienvenue !</h1>
     
      <p class="text-base text-center px-2 md:px-5 py-8 md:py-10">
        Groupomania est heureux de vous présenter son réseau social.<br />
        Nous avons mis en place cette plateforme afin que vous puissiez échanger
        entre collaborateurs sur divers sujets, et suivre toutes les actualités
        de notre groupe.<br />
        Pour cela il suffit de vous connecter, ou de vous inscrire si cela n'est
        pas déjà fait 🙂
      </p>
      <button
        @click="toLogin()"
        class="bg-gray-500 hover:bg-green-500 hover:shadow-xl text-white font-bold py-2 px-4 rounded-md"
      >
        Déjà inscrit ?
      </button>
      <button
        @click="toSignup()"
        class="bg-gray-500 hover:bg-green-500 hover:shadow-xl text-white font-bold py-2 px-4 mt-6 rounded-md"
      >
        S'inscrire
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
  methods: {
    // Utilisation d'instances router pour créer des ancres
    toLogin() {
      this.$router.push({ path: "/login" });
    },
    toSignup() {
      this.$router.push({ path: "/signup" });
    },
  },
};
</script>
