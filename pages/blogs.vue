<template>
  <div>
    <v-layout row wrap>
      <v-flex xs4>
        <v-card v-for="(post, i) in page" :key="i" outlined>
          <v-card-title primary-title>
            <nuxt-link to="/post" para>
              {{post.fields.title}}
            </nuxt-link>
          </v-card-title>
          <v-card-text>
            {{post.fields.description}}
          </v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
import { createClient } from "../plugins/contentful";
const contentfulClient = createClient();

export default {
  asyncData() {
    return contentfulClient
      .getEntries()
      .then(pages => {
        console.log(pages);
        return {
          page: pages.items
        };
      })
      .catch(console.error);
  }
};
</script>
