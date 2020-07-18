<template>
<div>
  <v-layout justify-center class="mt-10">
    <v-flex
      xs12
      md6
    >
    <h1 class="mt-4">Introduction</h1>
    <h3 class="mb-4">By Sajib Hawee</h3>
    <article>
      Computer Science has been an interest of mine since the day I discovered this subject.
      And the subject has brought me to Frontend Development.
      I have been working with <a href="https://vuejs.org/">Vue.js</a> from the start after migrating to it
      from <a href="https://reactjs.org/">React.js</a>.
    </article>

    <article class="mt-2">
      I have enthusiasm to work with other technologies as I have already worked with express, C#(WPF, WF),
      mongodb, python. My goal is to make contributions to open source projects and write some articles for 
      new developers about my mistakes and places where I was stuck.
    </article>

    </v-flex>
  </v-layout>
  <v-layout justify-center>
    <v-flex xs12 md6>

    <footer class="mt-10 social_icon">
      <a href="https://www.linkedin.com/in/sajib-hawee-2a818b154/" target="_blank">
        <font-awesome-icon :icon="['fab', 'linkedin']"/>
      </a>
      <a href="https://github.com/haweecodes" target="_blank">
        <font-awesome-icon :icon="['fab', 'github']"/>
      </a>
      <a href="https://www.facebook.com/haweeinthezone/" target="_blank">
        <font-awesome-icon :icon="['fab', 'facebook']"/>
      </a>
    </footer>
    </v-flex>
  </v-layout>
</div>
</template>

<script>
export default {
  transition: 'home',
  head () {
    return {
      title: 'Me | iamHawee.io',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: '' }
      ]
    }
  }
}
</script>

<style>
.home-enter-active, .home-leave-active {
    position: absolute;
    max-width:725.328px; /*make sur our content keep it's original width*/
    transition: all .2s ease;
  }

  /* entering start */  
  .home-enter {
    left: -100%;
  }

  /* entering end */
  .home-enter-to {
    left: 0;
  }

  /* leaving start */
  .home-leave {
    opacity: 1;
  }

  /* leaving end */
  .home-leave-to {
    opacity: 0;
  }
h1,
h3,
article {
  font-family: 'Nunito', sans-serif;
}
.social_icon{
  font-size: 28px;
  display: flex;
  justify-content: center;
}

footer a {
  text-decoration: none;
  color: black !important;
  margin: 0 10px 0 10px;
}
</style>
