<template>
  <v-layout class="mt-10" row wrap>
    <v-flex xs12>
      <h1 class="mt-4">Github Work</h1>
      <h3 class="mb-4">By Sajib Hawee</h3>
    </v-flex>
    <v-flex xs12 md6>
      <v-card outlined>
        <v-card-title>
          <a href="https://github.com/haweecodes/image-resize" class="company_links" target="_blank">Image Resize</a>
        </v-card-title>
        <v-card-subtitle><a href="https://haweecodes.github.io/image-resize/" target="_blank" rel="noopener noreferrer">Demo Here</a></v-card-subtitle>
        <v-card-text>
         This is my first work with canvas. This small app will resize any of your Icon beign (1024 x 1024) to icons with smaller dimesions.
         This works are the excitement that made me more interested in frontend development. Its not always get this and show that.
         This shows frontend can be a standalone app without any need for backend. Will be migrating this to a proper app with React/Vue.
        </v-card-text>
      </v-card>
    </v-flex>
    <v-flex xs12 md6>
      <v-card outlined>
        <v-card-title>
          <a href="https://github.com/haweecodes/vue-shadowbox" class="company_links" target="_blank">Vue ShadowBox</a>
        </v-card-title>
        <v-card-text>
          A lightbox library for Vue. Named it shadowbox cause there are lots of lightbox 😛.
          I was inspired by many developers making lightbox sample for react.
          I thought why not try to make one for Vue plus I can have a project for my portfolio.
          Its in <a href="https://www.npmjs.com/package/vue-shadowbox">npm</a> try it out and give a feedback pls.
        </v-card-text>
      </v-card>
    </v-flex>
    <v-flex xs12 md6>
      <v-card outlined>
        <v-card-title>
          <a href="https://github.com/haweecodes/HighLevel_demo" class="company_links" target="_blank">Page Builder</a>
        </v-card-title>
        <v-card-subtitle><a href="https://wizardly-lumiere-dcbf92.netlify.app/">Demo Here</a></v-card-subtitle>
        <v-card-text>
          This was a interview task I had to do for a company named HighLevel. I thought about working with it but couldn't have
          the time to concentrate and really work on it. I'm hoping I will work with this in the future maybe with React.
        </v-card-text>
      </v-card>
    </v-flex>
        <v-flex xs12 md6>
      <v-card outlined>
        <v-card-title>
          <a href="https://github.com/haweecodes/react-express-graphql" class="company_links" target="_blank">React GraphQL served by Express with GraphQL</a>
        </v-card-title>
        <v-card-text>
          Okay so the title seems confusing. What I did was use express to serve a react app which uses graphql to communicate with api from the express made with graphql.
          My first time using GraphQl and worked with react after a long time so peace.
        </v-card-text>
      </v-card>
    </v-flex>

    <v-flex xs12>
      <h1 class="mt-4">CodePen Scribbles</h1>
      <h3 class="mb-4">By Sajib Hawee</h3>
    </v-flex>
    <v-flex xs12 md6>
        <v-card outlined>
        <v-card-title>
          A strawhat design with sass
        </v-card-title>
        <v-card-subtitle><a href="https://codepen.io/haweecodes/pen/wLNbOe" target="_blank" rel="noopener noreferrer">Pen Here</a></v-card-subtitle>
        <v-card-text>
         <p class="codepen" data-height="265" data-theme-id="dark" data-default-tab="result" data-user="haweecodes" data-slug-hash="wLNbOe" data-preview="true" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="StrawHat">
          <span>See the Pen <a href="https://codepen.io/haweecodes/pen/wLNbOe">
          StrawHat</a> by Sajib Hawee (<a href="https://codepen.io/haweecodes">@haweecodes</a>)
          on <a href="https://codepen.io">CodePen</a>.</span>
        </p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
        </v-card-text>
      </v-card>
      <p></p>
      
    </v-flex>
    <v-flex xs12 md6>
        <v-card outlined>
        <v-card-title>
          Loading effect
        </v-card-title>
        <v-card-subtitle><a href="https://codepen.io/haweecodes/pen/dBwaZP" target="_blank" rel="noopener noreferrer">Pen Here</a></v-card-subtitle>
        <v-card-text>
         <p class="codepen" data-height="265" data-theme-id="dark" data-default-tab="result" data-user="haweecodes" data-slug-hash="dBwaZP" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="Text loading">
          <span>See the Pen <a href="https://codepen.io/haweecodes/pen/dBwaZP">
          Text loading</a> by Sajib Hawee (<a href="https://codepen.io/haweecodes">@haweecodes</a>)
          on <a href="https://codepen.io">CodePen</a>.</span>
        </p>
        <script async src="https://static.codepen.io/assets/embed/ei.js"></script>
        </v-card-text>
      </v-card>
      <p></p>
      
    </v-flex>

    

  </v-layout>
</template>

<script>
export default {
  transition: 'work',
  head () {
    return {
      title: 'Work | iamHawee.io',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: '' }
      ]
    }
  }
}
</script>

<style>
.work-enter-active, .work-leave-active {
    position: absolute;
    max-width:725.328px; /*make sur our content keep it's original width*/
    transition: all .2s ease;
  }

  /* entering start */  
  .work-enter {
    right: -100%;
  }

  /* entering end */
  .work-enter-to {
    right: 0;
  }

  /* leaving start */
  .work-leave {
    opacity: 1;
  }

  /* leaving end */
  .work-leave-to {
    opacity: 0;
  }
.company_links {
  text-decoration: none;
}
</style>