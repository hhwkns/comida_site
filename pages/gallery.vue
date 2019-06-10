<template>
    <section>
      <top />
      <div class="intro">
        <h1>Gallery</h1>
        <p class="lead">Oaxaca is known in culinary circles for its unique and wonderfully spicy dishes. Our food reflects centuries of tradition and culture.</p>
      </div>
      <div class="gallery">
       <b-img v-bind="mainProps" src="~/assets/food4.jpg" rounded alt="our restaurant"></b-img>
       <b-img v-bind="mainProps" src="~/assets/edgar-castrejon.jpg" rounded alt="fresh tacos"></b-img>
       <b-img v-bind="mainProps" src="~/assets/food1.jpg" rounded alt="camarones con rojo"></b-img>
       <b-img v-bind="mainProps" src="~/assets/karly-gomez.jpg" rounded alt="huevos ranchero"></b-img>
       <b-img v-bind="mainProps" src="~/assets/food6.jpg" rounded alt="fresh steak and tacos"></b-img>
       <b-img v-bind="mainProps" src="~/assets/food3.jpg" rounded alt="chips with homemade guacomole"></b-img>
      </div>

    <!-- <div class="gallery" v-for="image in gallery">
        <img class="img" v-bind:src="image.picture" v-bind:alt="image.alt">
      </div> -->
    </div>
    <bottom />
</section>
</template>

<script>
import top from '~/components/top.vue'
import bottom from '~/components/bottom.vue'

export default {
  components: {
    top,
    bottom
  },
  data () {
  return {
         mainProps: {
           blank: false,
           blankColor: '#777',
           width: 350,
           height: 350,
           class: 'm1'
         }
       }
}
//   gallery:[
//     { picture: require('~/assets/food4.jpg'), alt:'our restaurant' },
//     { picture: require('~/assets/edgar-castrejon.jpg'), alt:'fresh tacos' },
//     { picture: require('~/assets/food1.jpg'), alt:'camarones con rojo' },
//     { picture: require('~/assets/karly-gomez.jpg'), alt:'huevos rancheros' },
//     { picture: require('~/assets/food6.jpg'), alt:'fresh steak and tacos' },
//     { picture: require('~/assets/food3.jpg'), alt:'chips with homemade guacomole' }
//   ],
//   }
// }
}
</script>

<style lang="css">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
  font-size: 5em;
}

ul, .footer {
  list-style-type: none;
  padding: 1rem;
    background-color: #ACD143;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

p {
  justify: center;
}

.gallery {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  flex-wrap: wrap;
  align-content: stretch;
}

img {
  object-fit: cover;
  margin: 2rem;
}

</style>
