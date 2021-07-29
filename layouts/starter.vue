<template>
  <section>
    <div class="wrapper d-flex align-items-stretch">
      <transition name="slide-fade" mode="out-in">
        <component :is="sideBar"></component>
      </transition>
      <!-- Page Content  -->
      <div id="content" class="p-3">
        <nav
          class="
            navbar navbar-expand-lg navbar-light
            bg-light
            shadow
            p-3
            mb-5
            bg-white
            rounded
          "
        >
          <div class="container-fluid">
            <button type="button" id="sidebarCollapse" @click="toggle" class="btn btn-primary">
              <i class="fa fa-bars"></i>
              <span class="sr-only">Toggle Menu</span>
            </button>

            <button class="btn btn-primary">Title</button>

            <button
              class="btn btn-primary"
              data-toggle="modal"
              data-target="#exitModal"
            >
              <i class="fa fa-sign-out"></i>
            </button>
          </div>
        </nav>
        
        <Nuxt />
      </div>
    </div>
  </section>
</template>     

<script>
import SideBar from "@/components/layout/SideBar";
export default {
  components: {
    SideBar,
  },
  data() {
    return {
      sideBar: "SideBar",
    };
  },
  methods: {
    toggle() {
      if (this.sideBar === "SideBar") {
        this.sideBar = "";
      } else {
        this.sideBar = "SideBar";
      }
    },
  },
};
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}
.slide-fade-leave-active {
  transition: all 0.3s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */ {
  transform: translateX(10px);
  opacity: 0;
}
</style>