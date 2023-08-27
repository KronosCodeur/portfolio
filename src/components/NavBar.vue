<template>
  <v-app-bar app class="px-12" :color="color" dark flat >
    <v-btn>
      <v-icon class="mr-2" color="#01AF49" left>fas fa-signature</v-icon>
      Kronos Codeur
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn :class="{'text-green-accent-3':selectedItem==='home'}" text @click="scroll('home')">Accueil</v-btn>
    <v-btn :class="{'text-green-accent-3':selectedItem==='about'}" text @click="scroll('about')">Qui suis-je?</v-btn>
    <v-btn :class="{'text-green-accent-3':selectedItem==='services'}" text @click="scroll('services')">Services</v-btn>
    <v-btn :class="{'text-green-accent-3':selectedItem==='portfolio'}" text @click="scroll('portfolio')">Portfolio</v-btn>
    <v-btn>Blog</v-btn>
    <v-btn :class="{'text-green-accent-3':selectedItem==='contact'}" text @click="scroll('contact')">Contact</v-btn>
  </v-app-bar>
</template>
<script>
export default {
  data: () => ({
    selectedItem: 'home',
    sections: ['home', 'about', 'services', 'portfolio', 'contact']
  }),
  methods: {
    scroll(refName) {
      this.selectedItem=refName;
      const element = document.getElementById(refName);
      element.scrollIntoView({behavior: "smooth"})
    }
  },
  computed: {
    color() {
      // replace `true` and `false` with your condition
      return this.selectedItem==='home' ? '#0A0E11' : '#161e23';
    },
  },
  mounted() {
    this.$nextTick(() => {
      const observer = new IntersectionObserver(
          (entries) => {
            entries.forEach((entry) => {
              if (entry.isIntersecting) {
                this.selectedItem = entry.target.id;
              }
            });
          },
          { threshold: 0.7 }
      );
      this.sections.forEach((section) => {
        const element = document.getElementById(section);
        if (element) {
          observer.observe(element);
        }
      });
    });
  },
}
</script>
<style scoped>
</style>