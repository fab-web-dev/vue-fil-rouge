<template>
  <section class="section section-split section-hide-lc">
        <h2 class="section-title">Articles populaires</h2>
        <div class="section-container">
            <article class="article" v-for="(article) in articles" :key="article.id">
                <a href="#" class="article-link">
                    <figure class="article-figure">
                        <img class="article-img" :src="article.img" :alt="article.title">
                        <figcaption class="article-figcaption">{{article.title}}</figcaption>
                    </figure>
                </a>
            </article>
        </div>
    </section>
</template>

<script>
import axios from 'axios';

export default {
    data() {
        return {
            articles: []
        }
    },
    mounted() {
    axios
      .get('/json/articles.json')
      .then(response => this.articles = response.data)
  }
}
</script>

<style>

</style>