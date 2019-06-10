<template>
  <section>
    <top />
    <div class="intro">
     <h1>Our Story</h1>
      <p class="lead">Our story begins in Oaxaca, Mexico in 1998, when Chef
        Ronaldo discovered his love of food.</p>
    </div>
    <div class="chef">
      <div class="text">
        <h3>Chef Ronaldo</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit,
          sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat.Lorem ipsum dolor sit amet, consectetur adipiscing elit,
          sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat</p>
          <a href="mailto:hhwkns@gmail.com"><button class="btn">Contact Us</button></a>
        </div>
      <div class="image">
          <img src="~/assets/yucel-moran.jpg" alt="Chef Ronaldo" class="img">
      </div>
    </div>
    <div class="location">
      <h3>Location &amp; Hours</h3>
    <h4>Hours</h4>
      <p>Closed Monday <br>
      Tuesday - Saturday: 4 p.m. - Midnight <br>
      Sunday: Noon - 9 p.m.</p>
    <h4>Location</h4>
      <p>1325 4th Ave <br>
      Seattle, WA 98101 <br>
      (206) 618-8112  <br>
      <a href="mailto:oaxacateam@gmail.com">oaxacateam@gmail.com</a></p>

      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2689.8935263721337!2d-122.33806724892393!3d47.60875997908256!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54906ab3929838e7%3A0xf2583472d9632475!2s1325+4th+Ave+%23400%2C+Seattle%2C+WA+98101!5e0!3m2!1sen!2sus!4v1559605042342!5m2!1sen!2sus" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
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
  }
};
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

h4 {
  font-style: italic;
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

.btn {
  padding: .5rem;
  margin: .5rem;
  border-radius: 2px;
  background-color: gray;
  color: white;
  font-style: bold;
}

.chef {
  display: flex;
    &__image {
      object-fit: covoer;
      align-self: flex-start;
      flex-wrap: wrap;
  }
}

.img {
  width: 350px;
  height: 350px;
  margin: 1rem;
  padding: 1rem;
}

.text {
  margin: 1rem;
}

.location {
  position: relative;
  padding-bottom: 56.25%;
  padding-top: 35px;
  height: 0;
  overflow: hidden;
  margin: 1rem;
}

.location i-frame {
  position: absolute;
  top: 0;
  left: 0;
  width: 100% !important;
  height: 100% !important;
}
</style>
