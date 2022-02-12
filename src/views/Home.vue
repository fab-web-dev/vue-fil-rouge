<template>
  <div class="banner" :style="backgroundBanner"></div>
  <div class="section-all">
    <LastArticle></LastArticle>
    <PopularArticle></PopularArticle>
  </div>
</template>

<script>
import LastArticle from '../components/LastArticle.vue';
import PopularArticle from '../components/PopularArticle.vue';
// @ is an alias to /src
export default {
  name: "Home",
  components: {
    LastArticle,
    PopularArticle
},
  data() {
      return {
        backgroundBanner: {
          backgroundImage: `url(${require('@/assets/headerphoto.jpeg')})`
        }
      }
    }
};
</script>
