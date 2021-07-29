<template>
  <nav id="sidebar" >
    <div class="p-4">
      <h1>
        <a href="index.html" class="logo"
          >Portfolic <span>Portfolio Agency</span></a
        >
      </h1>
      <ul class="list-unstyled components mb-5">
        <li class="active">
          <nuxt-link to="/" @click="{setAlert}"><span class="fa fa-home mr-3"></span> Home</nuxt-link>
        </li>
        <li >
          <nuxt-link to="/"><span class="fa fa-user mr-3"></span> Clients</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/"><span class="fa fa-briefcase mr-3"></span> Works</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/"><span class="fa fa-sticky-note mr-3"></span> Blog</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/"><span class="fa fa-suitcase mr-3"></span> Gallery</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/"><span class="fa fa-cogs mr-3"></span> Services</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/"><span class="fa fa-paper-plane mr-3"></span> Contacts</nuxt-link>
        </li>
      </ul>
      <div class="footer">
        <p>Copyright &copy;</p>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
    methods:{
        setAlert(){
            alert('slm');
        }
    }
};
</script>

<style scoped>
    .nuxt-link-active {
        color: red;
    }
</style>