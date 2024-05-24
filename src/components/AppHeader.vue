<script>
export default {
  data() {
    return {
      links: [
                {
                    text: "CHARACTERS",
                    url: "#characters",
                },
                {
                    text: "COMICS",
                    url: "#comics",
                },
                {
                    text: "MOVIES",
                    url: "#movies",
                },
                {
                    text: "TV",
                    url: "#tv",
                },
                {
                    text: "GAMES",
                    url: "#games",
                },
                {
                    text: "COLLECTIBLES",
                    url: "#collectibles",
                },
                {
                    text: "VIDEOS",
                    url: "#videos",
                },
                {
                    text: "FANS",
                    url: "#fans",
                },
                {
                    text: "NEWS",
                    url: "#news",
                },
                {
                    text: "SHOP",
                    url: "#shop",
                },
            ],

    }
  },
  methods: {
    
  },
  mounted() {
    
  }
}
</script>

<template>
  <header>
    <img src="/public/img/dc-logo.png" alt="">
        <a v-for="link in links" :href="link.url">{{ link.text }}</a>
    </header>
</template>

<style scoped>
header{
  background-color: white;
  display: flex;
  flex-direction: row;
  
}
img{
  margin-left: 15rem;
  margin-right: 15rem;
  width: 5rem;
}
a{
  text-decoration: none;
    margin: 1rem 1rem;
    font-size: 12px;
    font-weight: bold;
}
</style>
